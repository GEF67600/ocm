---
layout: default
title: Mexique
permalink: /pays/mexique/
---
<img src="{{ '/assets/images/mexique-carte.jpg' | relative_url }}" class="map-banner">
# Mexique

<div class="hero-card">
Le Mexique constitue aujourd’hui un centre stratégique du narcotrafic mondial, 
notamment dans la production synthétique (méthamphétamine, fentanyl) 
et l’exportation vers les États-Unis.
</div>

---

## Organisations majeures

<div class="cards">
{% for post in site.categories.organisations %}
  {% if post.content contains "Pays : Mexique" %}
  <div class="card">
    <div class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>

---

## Dirigeants clés

<div class="cards">
{% for post in site.categories.dirigeants %}
  {% if post.content contains "Mexique" or post.content contains "Cartel" %}
  <div class="card">
    <div class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>

---

## Mutation stratégique

<div class="hero-card">
Depuis 2015, le modèle économique évolue :

- Passage progressif vers les drogues synthétiques  
- Réduction de la dépendance aux cultures traditionnelles  
- Fragmentation structurelle des cartels  
- Montée en puissance du CJNG  

Le fentanyl représente aujourd’hui un facteur de pression diplomatique majeur.
</div>

---

## Chronologie

<a class="btn" href="{{ '/mexique/chronologie/' | relative_url }}">
Voir la chronologie complète
</a>

---

## Enjeux actuels

<div class="card">
- Militarisation du conflit interne  
- Corruption institutionnelle persistante  
- Pression judiciaire américaine  
- Recomposition permanente des factions
</div>
