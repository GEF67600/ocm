---
layout: default
title: Accueil
---

# Les Organisations Criminelles Mondiales (OCM)

Site de documentation : organisations, dirigeants, marchés, routes, méthodes, chronologies.

## Derniers articles
<div class="card">
  <ul>
    {% for post in site.posts limit:10 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        — <small>{{ post.date | date: "%d/%m/%Y" }}</small>
      </li>
    {% endfor %}
  </ul>
</div>
