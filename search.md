---
layout: default
title: Search
permalink: /search/
---

# Search

<input id="searchBox" type="text" placeholder="Search insights, glossary, field kits…" style="width:100%;padding:12px;border-radius:10px;border:1px solid #d9deea;font-size:16px;">

<div id="results" style="margin-top:18px;"></div>

<script>
(async function () {
  const results = document.getElementById('results');
  const box = document.getElementById('searchBox');

  function showError(msg) {
    results.innerHTML = `<div class="card"><p><strong>Search isn’t available yet.</strong><br>${msg}</p></div>`;
  }

  // Load Lunr (with a fallback error)
  try {
    const s = document.createElement('script');
    s.src = 'https://unpkg.com/lunr/lunr.js';
    s.onload = initSearch;
    s.onerror = () => showError('Could not load the search library (lunr.js). If your network blocks unpkg.com, we can host lunr locally in this repo.');
    document.head.appendChild(s);
  } catch (e) {
    showError(e.message);
  }

  async function initSearch() {
    try {
      const indexUrl = '{{ "/search.json" | relative_url }}';
      const res = await fetch(indexUrl);
      if (!res.ok) throw new Error(`Could not load search index: ${res.status} ${res.statusText}`);

      const data = await res.json();
      if (!Array.isArray(data) || data.length === 0) throw new Error('Search index loaded, but it is empty.');

      const idx = lunr(function () {
        this.ref('id');
        this.field('title');
        this.field('content');
        this.field('tags');

        data.forEach(doc => this.add(doc));
      });

      function render(items) {
        if (!items.length) {
          results.innerHTML = '<p>No results.</p>';
          return;
        }

        results.innerHTML = items.map(i => {
          // Ref can be string; ids may be numeric — normalize:
          const d = data.find(x => String(x.id) === String(i.ref));
          if (!d) return '';

          return `
            <div class="card" style="margin:12px 0;">
              <h2 style="margin:0 0 6px;font-size:18px;">
                <a href="${d.url}">${d.title}</a>
              </h2>
              <p style="margin:0;">${d.excerpt || ""}</p>
            </div>
          `;
        }).join('') || '<p>No results.</p>';
      }

      box.addEventListener('input', () => {
        const q = box.value.trim();
        if (!q) { results.innerHTML = ''; return; }
        const found = idx.search(q).slice(0, 10);
        render(found);
      });

    } catch (err) {
      console.error(err);
      showError(err.message);
    }
  }
})();
</script>
