---
layout: default
title: Analyses
permalink: /analyses/
---

# Analyses

<div class="hero-card">
Articles de fond sur les structures criminelles, les mutations stratégiques, les routes et les modèles économiques.
</div>

<div class="cards">
{% assign posts = site.categories.analyses %}
{% for post in posts %}
  <div class="card">
    <div class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </div>
    <div class="muted">
      {{ post.date | date: "%d/%m/%Y" }}
    </div>
  </div>
{% endfor %}
</div>
