---
layout: default
title: Home
search: false
---

<section class="hero">
  <h1>Maven's Asset Performance Management Field Glossary</h1>
  <p><strong>IBM Maximo &amp; Enterprise Asset Management in Plain English.</strong> Asset management is complex enough without confusing language.</p>
</section>

<div class="grid">
  <section class="card">
    <h2>Latest Insights</h2>
    <p>Maven perspectives on Maximo, reliability strategy, and asset performance.</p>
    <ul>
      {% for post in site.posts limit:3 %}
        <li><strong>{{ post.date | date: "%B %Y" }}:</strong> <a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
    <div style="margin-top:14px;">
      <a class="button" href="{{ "/maven-insights" | relative_url }}">View all insights</a>
    </div>
  </section>

 <section class="card">
  <h2>Executive Glossary</h2>
  <p>A growing set of leadership-level definitions for Maximo and EAM concepts.</p>
  <a class="button" href="{{ "/glossary" | relative_url }}">View glossary</a>
</section>

  <section class="card">
    <h2>Field Kits &amp; Tools</h2>
    <p>Practical checklists and frameworks that translate strategy into execution.</p>
    <ul>
      <li>Fiscal Year End Maximo Updates checklists</li>
    </ul>
    <div style="margin-top:14px;">
      <a class="button" href="{{ "/field-kits" | relative_url }}">Explore kits</a>
    </div>
  </section>
</div>

<p class="section-title">Why we built this</p>
<div class="card">
  <p>Too often, organizations invest in systems like Maximo without shared clarity on what key concepts actually mean in practice, reliability that reduces surprise failures, governance that sustains standards, data leaders can trust, and work management that improves predictability.</p>
  <p>This site is designed to be useful.</p>
</div>
