---
layout: page
title: Blog de l'association
permalink: /blog/
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ page.date | date: '%d %B %Y' }}
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">En savoir plus...</a>
    </article>
  {% endfor %}
</div>
