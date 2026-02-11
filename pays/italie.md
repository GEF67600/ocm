---
layout: default
title: Italie
permalink: /pays/italie/
---

# Italie

<div class="hero-card">
Organisations et analyses liées à l’Italie.
</div>

<h2>Organisations</h2>
<div class="cards">
{% for post in site.categories.organisations %}
  {% if post.content contains "Pays : Italie" %}
  <div class="card">
    <div class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
    <div class="muted">{{ post.date | date: "%d/%m/%Y" }}</div>
  </div>
  {% endif %}
{% endfor %}
</div>

<h2>Analyses</h2>
<div class="cards">
{% for post in site.categories.analyses %}
  {% if post.content contains "Italie" %}
  <div class="card">
    <div class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
    <div class="muted">{{ post.date | date: "%d/%m/%Y" }}</div>
  </div>
  {% endif %}
{% endfor %}
</div>
