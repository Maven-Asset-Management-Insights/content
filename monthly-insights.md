---
layout: default
title: Monthly Insights
permalink: /monthly-insights/
---

# Maven Insights

<p>Maven perspectives on IBM Maximo, reliability strategy, and asset performance—written in plain English and grounded in outcomes.</p>

{% for post in site.posts %}
<div class="card post-card">

  <div class="post-meta">
    <strong>{{ post.date | date: "%B %d, %Y" }}</strong>
  </div>

  <h2 class="post-title">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h2>

  {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</p>
  {% endif %}

  {% if post.tags %}
  <div class="tags">
    {% for tag in post.tags %}
      <span class="tag">{{ tag }}</span>
    {% endfor %}
  </div>
  {% endif %}

</div>
{% endfor %}
