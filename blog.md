---
layout: page
title: Blog de la communauté
permalink: /blog/
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
      <time class="dt-published" datetime="{{post.date | date_to_xmlschema }}">
      {{ post.date | date: '%-d' }} {% assign m = post.date | date: "%-m" %}{% case m %}{% when '1' %}janv.{% when '2' %}févr.{% when '3' %}mars{% when '4' %}avr.{% when '5' %}mai{% when '6' %}juin{% when '7' %}juil.{% when '8' %}août{% when '9' %}sept.{% when '10' %}oct.{% when '11' %}nov.{% when '12' %}déc.{% endcase %} 
    {{ post.date | date: '%Y' }}  
      </time>
      
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">En savoir plus...</a>
    </article>
  {% endfor %}
</div>
