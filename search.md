---
layout: default
title: Search
permalink: /search/
---

# Search

<input id="searchBox" type="text" placeholder="Search insights, glossary, field kits…" style="width:100%;padding:12px;border-radius:10px;border:1px solid #d9deea;font-size:16px;">

<div id="results" style="margin-top:18px;"></div>

<script src="https://unpkg.com/lunr/lunr.js"></script>
<script>
(async function () {
  const res = await fetch('{{ "/search.json" | relative_url }}');
  const data = await res.json();

  const idx = lunr(function () {
    this.ref('id');
    this.field('title');
    this.field('content');
    this.field('tags');

    data.forEach(doc => this.add(doc));
  });

  const box = document.getElementById('searchBox');
  const results = document.getElementById('results');

  function render(items) {
    if (!items.length) {
      results.innerHTML = '<p>No results.</p>';
      return;
    }
    results.innerHTML = items.map(i => {
      const d = data.find(x => x.id === i.ref);
      return `
        <div class="card" style="margin:12px 0;">
          <h2 style="margin:0 0 6px;font-size:18px;">
            <a href="${d.url}">${d.title}</a>
          </h2>
          <p style="margin:0;">${d.excerpt}</p>
        </div>
      `;
    }).join('');
  }

  box.addEventListener('input', () => {
    const q = box.value.trim();
    if (!q) { results.innerHTML = ''; return; }
    const found = idx.search(q).slice(0, 10);
    render(found);
  });
})();
</script>
