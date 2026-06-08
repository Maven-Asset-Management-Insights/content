---
layout: default
title: Home
search: false
---
<section class="hero">
  <h1>Know the Language. Lead the Initiative.</h1>
  <h2>Maven's Field Glossary for Maximo and EAM Leaders</h2>
<div class="video-container" style="max-width: 600px; margin: 1.5rem auto 2rem auto; padding-bottom: 40%;">
  <iframe
    src="https://www.youtube.com/embed/bMbEX0IYHe8"
    title="Maven Asset Performance Management Field Glossary Overview"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>
  <p><strong>IBM Maximo &amp; Enterprise Asset Management Clearly Explained: Asset management is challenging enough without adding unnecessary complexity.</strong></p>
  <p style="margin-top: 1rem;">Maven works with organizations to turn this knowledge into outcomes. <a href="https://www.mavenasset.com">See how Maven can help.</a></p>
</section>

<div class="grid">

  <!-- ── INSIGHTS ── -->
  <section class="card" style="padding:0; overflow:hidden;">
    <svg width="100%" height="140" viewBox="0 0 680 200" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Latest Insights</title>
      <desc>Maven branded header for the Latest Insights section</desc>
      <defs><marker id="arr-ins" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse"><path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></marker></defs>
      <rect width="680" height="200" fill="#292C75"/>
      <rect x="0" y="0" width="7" height="200" fill="#3E67B1"/>
      <rect x="0" y="190" width="680" height="10" fill="#3E67B1"/>
      <text x="64" y="82" font-family="Arial Black, Arial" font-weight="900" font-size="42" fill="#FFFFFF" letter-spacing="1">INSIGHTS</text>
      <text x="64" y="116" font-family="Arial" font-size="20" fill="#A8C0E0">Maven perspectives on Maximo,</text>
      <text x="64" y="142" font-family="Arial" font-size="20" fill="#A8C0E0">reliability &amp; asset performance.</text>
      <circle cx="590" cy="96" r="52" fill="#3E67B1" opacity="0.22"/>
      <circle cx="590" cy="96" r="38" fill="none" stroke="#3E67B1" stroke-width="2" opacity="0.5"/>
      <polyline points="548,128 568,104 584,116 604,82 624,64" fill="none" stroke="#FFFFFF" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" marker-end="url(#arr-ins)"/>
      <circle cx="548" cy="128" r="4" fill="#A8C0E0"/>
      <circle cx="568" cy="104" r="4" fill="#A8C0E0"/>
      <circle cx="584" cy="116" r="4" fill="#A8C0E0"/>
      <circle cx="604" cy="82" r="4" fill="#A8C0E0"/>
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
    <svg width="100%" height="140" viewBox="0 0 680 200" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Glossary</title>
      <desc>Maven branded header for the Glossary section</desc>
      <rect width="680" height="200" fill="#3E67B1"/>
      <rect x="0" y="0" width="7" height="200" fill="#FFFFFF" opacity="0.3"/>
      <rect x="0" y="190" width="680" height="10" fill="#292C75"/>
      <text x="64" y="82" font-family="Arial Black, Arial" font-weight="900" font-size="42" fill="#FFFFFF" letter-spacing="1">GLOSSARY</text>
      <text x="64" y="116" font-family="Arial" font-size="20" fill="#C8DCF4">Leadership-level definitions for</text>
      <text x="64" y="142" font-family="Arial" font-size="20" fill="#C8DCF4">Maximo and EAM concepts.</text>
      <circle cx="580" cy="100" r="60" fill="#292C75" opacity="0.2"/>
      <circle cx="580" cy="100" r="42" fill="none" stroke="#FFFFFF" stroke-width="1" opacity="0.2"/>
      <text x="580" y="88" font-family="Arial Black, Arial" font-weight="900" font-size="36" fill="#FFFFFF" opacity="0.25" text-anchor="middle">A–Z</text>
      <text x="580" y="122" font-family="Arial" font-size="18" fill="#C8DCF4" opacity="0.5" text-anchor="middle">EAM defined</text>
    </svg>
    <div style="padding: 1.25rem 1.5rem 1.5rem;">
      <h2>Glossary</h2>
      <p>A growing set of leadership-level definitions for Maximo and EAM concepts.</p>
      <ul>
        <li><a href="{{ '/glossary/#asset-criticality' | relative_url }}">Asset Criticality</a></li>
        <li><a href="{{ '/glossary/#backlog-health' | relative_url }}">Backlog Health</a></li>
        <li><a href="{{ '/glossary/#condition-based-maintenance-cbm' | relative_url }}">Condition-Based Maintenance (CBM)</a></li>
        <li><a href="{{ '/glossary/#data-governance' | relative_url }}">Data Governance</a></li>
        <li><a href="{{ '/glossary/#enterprise-asset-management-eam' | relative_url }}">Enterprise Asset Management (EAM)</a></li>
        <li><a href="{{ '/glossary/#failure-mode' | relative_url }}">Failure Mode</a></li>
        <li><a href="{{ '/glossary/#internet-of-things-iot' | relative_url }}">Internet of Things (IoT)</a></li>
        <li><a href="{{ '/glossary/#job-plan' | relative_url }}">Job Plan</a></li>
        <li><a href="{{ '/glossary/#key-performance-indicator-kpi' | relative_url }}">Key Performance Indicator (KPI)</a></li>
        <li><a href="{{ '/glossary/#work-order-wo' | relative_url }}">Work Order (WO)</a></li>
      </ul>
      <div class="card-cta">
        <a class="button" href="{{ "/glossary" | relative_url }}">View full glossary</a>
      </div>
    </div>
  </section>

  <!-- ── FIELD KITS ── -->
  <section class="card" style="padding:0; overflow:hidden;">
    <svg width="100%" height="140" viewBox="0 0 680 200" role="img" xmlns="http://www.w3.org/2000/svg" style="display:block;">
      <title>Field Kits and Tools</title>
      <desc>Maven branded header for the Field Kits and Tools section</desc>
      <rect width="680" height="200" fill="#292C75"/>
      <rect x="0" y="0" width="7" height="200" fill="#3E67B1"/>
      <rect x="673" y="0" width="7" height="200" fill="#3E67B1"/>
      <rect x="0" y="190" width="680" height="10" fill="#3E67B1"/>
      <text x="64" y="78" font-family="Arial Black, Arial" font-weight="900" font-size="38" fill="#FFFFFF" letter-spacing="1">FIELD KITS</text>
      <text x="64" y="118" font-family="Arial Black, Arial" font-weight="900" font-size="38" fill="#FFFFFF" letter-spacing="1">&amp; TOOLS</text>
      <text x="64" y="150" font-family="Arial" font-size="20" fill="#A8C0E0">Practical frameworks that translate</text>
      <text x="64" y="174" font-family="Arial" font-size="20" fill="#A8C0E0">strategy into execution.</text>
      <rect x="484" y="52" width="18" height="18" rx="3" fill="none" stroke="#FFFFFF" stroke-width="2" opacity="0.8"/>
      <line x1="488" y1="61" x2="492" y2="66" stroke="#A8C0E0" stroke-width="2" stroke-linecap="round"/>
      <line x1="492" y1="66" x2="500" y2="55" stroke="#A8C0E0" stroke-width="2" stroke-linecap="round"/>
      <line x1="514" y1="61" x2="628" y2="61" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" opacity="0.5"/>
      <rect x="484" y="85" width="18" height="18" rx="3" fill="none" stroke="#FFFFFF" stroke-width="2" opacity="0.8"/>
      <line x1="488" y1="94" x2="492" y2="99" stroke="#A8C0E0" stroke-width="2" stroke-linecap="round"/>
      <line x1="492" y1="99" x2="500" y2="88" stroke="#A8C0E0" stroke-width="2" stroke-linecap="round"/>
      <line x1="514" y1="94" x2="628" y2="94" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" opacity="0.5"/>
      <rect x="484" y="118" width="18" height="18" rx="3" fill="none" stroke="#FFFFFF" stroke-width="2" opacity="0.8"/>
      <line x1="514" y1="127" x2="600" y2="127" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" opacity="0.3"/>
    </svg>
    <div style="padding: 1.25rem 1.5rem 1.5rem;">
      <h2>Field Kits &amp; Tools</h2>
      <p>Practical checklists and frameworks that translate strategy into execution.</p>
      <ul>
        <li><a href="{{ '/field-kits/maximo-upgrade-process/' | relative_url }}">The Maximo Upgrade Process</a></li>
        <li><a href="{{ '/field-kits/maximo-readiness-scorecard.html' | relative_url }}">Maximo Readiness Scorecard</a></li>
        <li><a href="{{ '/field-kits/year-end-maximo/' | relative_url }}">Year-End Maximo Preparation</a></li>
        <li><a href="{{ '/field-kits/maintenance-goes-mobile-clarios/' | relative_url }}">Maintenance Goes Mobile (Clarios)</a></li>
        <li><a href="{{ '/field-kits/monitor-demo-practical-path-to-deployment/' | relative_url }}">Monitor Demo and Practical Path to Deployment</a></li>
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
