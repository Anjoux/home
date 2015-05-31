---
layout: page
title: Qui sommes nous ?
permalink: /about/
---

Quelques informations sur l'association !

### Comment y adhérer ?

A place to include any other types of information that you'd like to include about yourself.

### Contactez nous

[bonjour@anjoux.eu.org](mailto:bonjour@anjoux.eu.org)

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">En savoir plus...</a>
    </article>
  {% endfor %}
</div>
