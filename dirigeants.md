---
layout: default
title: Dirigeants
permalink: /dirigeants/
---

# Dirigeants

<div class="hero-card">
Liste des profils de dirigeants (chefs, lieutenants, fondateurs, figures clés).
</div>

<div class="cards">
{% assign posts = site.categories.dirigeants %}
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
