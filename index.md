---
layout: default
title: Accueil
---

<div class="hero">

  <div class="hero-left">

    <div class="kicker">OCM</div>

    <h1>Les Organisations Criminelles Mondiales</h1>

    <p class="lead">
      Site de documentation dédié aux organisations criminelles mondiales :
      structures, dirigeants, zones d’influence, modèles économiques et évolutions.
    </p>

    <div class="hero-actions">
      <a class="btn" href="{{ '/organisations/' | relative_url }}">Organisations</a>
      <a class="btn btn-ghost" href="{{ '/archive/' | relative_url }}">Analyses</a>
    </div>

    <div class="chips">
      <span class="chip">Mexique</span>
      <span class="chip">Colombie</span>
      <span class="chip">Europe</span>
      <span class="chip">Asie</span>
    </div>

  </div>

  <div class="hero-right">

    <div class="hero-card">
      <div class="hero-card-title">Derniers articles</div>

      <ul class="clean">
        {% for post in site.posts limit:6 %}
          <li>
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            <span class="muted">— {{ post.date | date: "%d/%m/%Y" }}</span>
          </li>
        {% endfor %}
      </ul>

    </div>

  </div>

</div>

<div class="section">
  <h2>À lire maintenant</h2>

  <div class="cards">
    {% for post in site.posts limit:3 %}
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

</div>
