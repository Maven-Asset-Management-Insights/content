---
layout: default
title: Home
search: false
---

<section class="hero">
  <h1>Maven's Asset Performance Management Field Glossary</h1>
  <p><strong>IBM Maximo & Enterprise Asset Management Clearly Explained: Asset management is challenging enough without adding unnecessary complexity.</strong></p>
</section>

<div class="grid">
  <section class="card">
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
  </section>

 <section class="card">
  <h2>Glossary</h2>
  <p>A growing set of leadership-level definitions for Maximo and EAM concepts.</p>

  <ul>
    <li><a href="{{ '/glossary/#asset-criticality' | relative_url }}">Asset Criticality</a></li>
    <li><a href="{{ '/glossary/#asset-health-index-ahi' | relative_url }}">Asset Health Index (AHI)</a></li>
    <li><a href="{{ '/glossary/#asset-hierarchy' | relative_url }}">Asset Hierarchy</a></li>
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
</section>

  <section class="card">
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
  </section>
</div>

<p class="section-title">Why we built this</p>
<div class="card">
  <p>
    We built this site to help organizations grow with clarity and confidence in Maximo by strengthening reliability, governance, trusted data, and predictable work management. A maven is an experienced expert who helps others grow, and this resource is designed to do exactly that: align teams, elevate understanding, and turn asset management into measurable performance.
  </p>
</div>
