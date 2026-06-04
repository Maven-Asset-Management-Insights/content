---
layout: default
title: Home
search: false
---
<section class="hero">
  <h1>Maven's Asset Performance Management Field Glossary</h1>
  <h2>Start here. What Is the Maven Field Glossary Resource Hub?</h2>
<div class="video-container" style="max-width: 600px; margin: 1.5rem auto 2rem auto; padding-bottom: 40%;">
  <iframe
    src="https://www.youtube.com/embed/bMbEX0IYHe8"
    title="Maven Asset Performance Management Field Glossary Overview"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>
  <p><strong>IBM Maximo & Enterprise Asset Management Clearly Explained: Asset management is challenging enough without adding unnecessary complexity.</strong></p>
</section>

<div class="grid">

  <!-- ── INSIGHTS ── -->
  <section class="card" style="padding:0; overflow:hidden;">
    <svg width="100%" viewBox="0 0 680 160" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Latest Insights</title>
      <desc>Maven branded header for the Latest Insights section</desc>
      <defs><marker id="arr-ins" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse"><path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></marker></defs>
      <rect width="680" height="160" fill="#292C75"/>
      <rect x="0" y="0" width="6" height="160" fill="#3E67B1"/>
      <rect x="0" y="152" width="680" height="8" fill="#3E67B1"/>
      <rect x="40" y="28" width="280" height="104" rx="8" fill="#3E67B1" opacity="0.18"/>
      <text x="64" y="72" font-family="Arial Black, Arial" font-weight="900" font-size="32" fill="#FFFFFF" letter-spacing="1">INSIGHTS</text>
      <text x="64" y="100" font-family="Arial" font-size="13" fill="#A8C0E0">Maven perspectives on Maximo,</text>
      <text x="64" y="118" font-family="Arial" font-size="13" fill="#A8C0E0">reliability strategy, and asset performance.</text>
      <circle cx="570" cy="76" r="44" fill="#3E67B1" opacity="0.22"/>
      <circle cx="570" cy="76" r="32" fill="none" stroke="#3E67B1" stroke-width="1.5" opacity="0.5"/>
      <polyline points="530,100 548,82 562,90 580,62 598,50" fill="none" stroke="#FFFFFF" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" marker-end="url(#arr-ins)"/>
      <circle cx="530" cy="100" r="3" fill="#A8C0E0"/>
      <circle cx="548" cy="82" r="3" fill="#A8C0E0"/>
      <circle cx="562" cy="90" r="3" fill="#A8C0E0"/>
      <circle cx="580" cy="62" r="3" fill="#A8C0E0"/>
      <rect x="40" y="148" width="40" height="3" rx="1.5" fill="#3E67B1"/>
      <rect x="88" y="148" width="20" height="3" rx="1.5" fill="#3E67B1" opacity="0.5"/>
      <rect x="116" y="148" width="10" height="3" rx="1.5" fill="#3E67B1" opacity="0.25"/>
    </svg>
    <div style="padding: 1.25rem 1.5rem 1.5rem;">
      <h2>Latest Insights</h2>
      <p>Maven perspectives on Maximo, reliability strategy, and asset performance.</p>
      <ul>
        {% for post in site.posts limit:5 %}
          <li>
            <strong>{{ post.date | date: "%B %-d, %Y" }}:</strong>
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </li>
        {% endfor %}
      </ul>
      <div style="margin-top:14px;">
        <a class="button" href="{{ "/maven-insights" | relative_url }}">View all insights</a>
      </div>
    </div>
  </section>

  <!-- ── GLOSSARY ── -->
  <section class="card" style="padding:0; overflow:hidden;">
    <svg width="100%" viewBox="0 0 680 160" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Glossary</title>
      <desc>Maven branded header for the Glossary section</desc>
      <rect width="680" height="160" fill="#3E67B1"/>
      <rect x="0" y="0" width="6" height="160" fill="#FFFFFF" opacity="0.3"/>
      <rect x="0" y="152" width="680" height="8" fill="#292C75"/>
      <rect x="40" y="28" width="280" height="104" rx="8" fill="#292C75" opacity="0.25"/>
      <text x="64" y="72" font-family="Arial Black, Arial" font-weight="900" font-size="32" fill="#FFFFFF" letter-spacing="1">GLOSSARY</text>
      <text x="64" y="100" font-family="Arial" font-size="13" fill="#C8DCF4">Leadership-level definitions for</text>
      <text x="64" y="118" font-family="Arial" font-size="13" fill="#C8DCF4">Maximo and EAM concepts.</text>
      <rect x="490" y="38" width="148" height="90" rx="6" fill="#292C75" opacity="0.3"/>
      <rect x="490" y="38" width="148" height="90" rx="6" fill="none" stroke="#FFFFFF" stroke-width="1" opacity="0.3"/>
      <text x="510" y="66" font-family="Arial" font-weight="700" font-size="13" fill="#FFFFFF" opacity="0.9">A</text>
      <text x="524" y="66" font-family="Arial" font-size="12" fill="#C8DCF4">Asset Criticality</text>
      <text x="510" y="84" font-family="Arial" font-weight="700" font-size="13" fill="#FFFFFF" opacity="0.9">F</text>
      <text x="524" y="84" font-family="Arial" font-size="12" fill="#C8DCF4">Failure Mode</text>
      <text x="510" y="102" font-family="Arial" font-weight="700" font-size="13" fill="#FFFFFF" opacity="0.9">M</text>
      <text x="524" y="102" font-family="Arial" font-size="12" fill="#C8DCF4">MTBF</text>
      <text x="510" y="120" font-family="Arial" font-weight="700" font-size="13" fill="#FFFFFF" opacity="0.9">R</text>
      <text x="524" y="120" font-family="Arial" font-size="12" fill="#C8DCF4">RCA</text>
      <rect x="40" y="148" width="40" height="3" rx="1.5" fill="#FFFFFF" opacity="0.4"/>
      <rect x="88" y="148" width="20" height="3" rx="1.5" fill="#FFFFFF" opacity="0.2"/>
      <rect x="116" y="148" width="10" height="3" rx="1.5" fill="#FFFFFF" opacity="0.1"/>
    </svg>
    <div style="padding: 1.25rem 1.5rem 1.5rem;">
      <h2>Glossary</h2>
      <p>A growing set of leadership-level definitions for Maximo and EAM concepts.</p>
      <ul>
        <li><a href="{{ '/glossary/#asset-criticality' | relative_url }}">Asset Criticality</a></li>
        <li><a href="{{ '/glossary/#asset-health-index-ahi' | relative_url }}">Asset Health Index (AHI)</a></li>
        <li><a href="{{ '/glossary/#asset-performance' | relative_url }}">Asset Performance</a></li>
        <li><a href="{{ '/glossary/#condition-based-maintenance-cbm' | relative_url }}">Condition-Based Maintenance (CBM)</a></li>
        <li><a href="{{ '/glossary/#enterprise-asset-management-eam' | relative_url }}">Enterprise Asset Management (EAM)</a></li>
        <li><a href="{{ '/glossary/#failure-code' | relative_url }}">Failure Code</a></li>
        <li><a href="{{ '/glossary/#failure-mode' | relative_url }}">Failure Mode</a></li>
        <li><a href="{{ '/glossary/#predictive-maintenance-pdm' | relative_url }}">Predictive Maintenance (PdM)</a></li>
      </ul>
      <div class="card-cta">
        <a class="button" href="{{ "/glossary" | relative_url }}">View full glossary</a>
      </div>
    </div>
  </section>

  <!-- ── FIELD KITS ── -->
  <section class="card" style="padding:0; overflow:hidden;">
    <svg width="100%" viewBox="0 0 680 160" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Field Kits and Tools</title>
      <desc>Maven branded header for the Field Kits and Tools section</desc>
      <rect width="680" height="160" fill="#292C75"/>
      <rect x="0" y="0" width="6" height="160" fill="#3E67B1"/>
      <rect x="674" y="0" width="6" height="160" fill="#3E67B1"/>
      <rect x="0" y="152" width="680" height="8" fill="#3E67B1"/>
      <rect x="40" y="28" width="280" height="104" rx="8" fill="#3E67B1" opacity="0.18"/>
      <text x="64" y="68" font-family="Arial Black, Arial" font-weight="900" font-size="26" fill="#FFFFFF" letter-spacing="1">FIELD KITS</text>
      <text x="64" y="94" font-family="Arial Black, Arial" font-weight="900" font-size="26" fill="#FFFFFF" letter-spacing="1">&amp; TOOLS</text>
      <text x="64" y="118" font-family="Arial" font-size="13" fill="#A8C0E0">Practical frameworks that translate</text>
      <text x="64" y="134" font-family="Arial" font-size="13" fill="#A8C0E0">strategy into execution.</text>
      <rect x="490" y="34" width="148" height="96" rx="6" fill="#3E67B1" opacity="0.25"/>
      <rect x="506" y="50" width="14" height="14" rx="2" fill="none" stroke="#FFFFFF" stroke-width="1.5" opacity="0.8"/>
      <line x1="509" y1="57" x2="512" y2="60" stroke="#A8C0E0" stroke-width="1.5" stroke-linecap="round"/>
      <line x1="512" y1="60" x2="518" y2="53" stroke="#A8C0E0" stroke-width="1.5" stroke-linecap="round"/>
      <line x1="528" y1="57" x2="622" y2="57" stroke="#FFFFFF" stroke-width="1.5" stroke-linecap="round" opacity="0.5"/>
      <rect x="506" y="72" width="14" height="14" rx="2" fill="none" stroke="#FFFFFF" stroke-width="1.5" opacity="0.8"/>
      <line x1="509" y1="79" x2="512" y2="82" stroke="#A8C0E0" stroke-width="1.5" stroke-linecap="round"/>
      <line x1="512" y1="82" x2="518" y2="75" stroke="#A8C0E0" stroke-width="1.5" stroke-linecap="round"/>
      <line x1="528" y1="79" x2="622" y2="79" stroke="#FFFFFF" stroke-width="1.5" stroke-linecap="round" opacity="0.5"/>
      <rect x="506" y="94" width="14" height="14" rx="2" fill="none" stroke="#FFFFFF" stroke-width="1.5" opacity="0.8"/>
      <line x1="528" y1="101" x2="590" y2="101" stroke="#FFFFFF" stroke-width="1.5" stroke-linecap="round" opacity="0.3"/>
      <rect x="40" y="148" width="40" height="3" rx="1.5" fill="#3E67B1"/>
      <rect x="88" y="148" width="20" height="3" rx="1.5" fill="#3E67B1" opacity="0.5"/>
      <rect x="116" y="148" width="10" height="3" rx="1.5" fill="#3E67B1" opacity="0.25"/>
    </svg>
    <div style="padding: 1.25rem 1.5rem 1.5rem;">
      <h2>Field Kits &amp; Tools</h2>
      <p>Practical checklists and frameworks that translate strategy into execution.</p>
      <ul>
        {% assign kits = site.pages
          | where_exp: "p", "p.url contains '/field-kits/'"
          | where_exp: "p", "p.url != '/field-kits/'"
          | sort: "date"
          | reverse %}
        {% for kit in kits limit:5 %}
          <li>
            <strong>{{ kit.date | date: "%B %-d, %Y" }}:</strong>
            <a href="{{ kit.url | relative_url }}">{{ kit.title }}</a>
          </li>
        {% endfor %}
      </ul>
      <div style="margin-top:14px;">
        <a class="button" href="{{ "/field-kits" | relative_url }}">Explore all kits</a>
      </div>
    </div>
  </section>

</div>

<p class="section-title">Why we built this</p>
<div class="card">
  <p>
    We built this site to help organizations grow with clarity and confidence in Maximo by strengthening reliability, governance, trusted data, and predictable work management. A maven is an experienced expert who helps others grow, and this resource is designed to do exactly that: align teams, elevate understanding, and turn asset management into measurable performance.
  </p>
</div>
