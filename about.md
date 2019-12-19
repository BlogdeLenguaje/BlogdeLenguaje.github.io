---
layout: default
title: Unidades
---
  <h1 class="pageTitle">Introduccion a la Ingenieria en Software</h1>
  <embed src="{{ '/assets/img/DBZindex.mp3' | prepend: site.baseurl }}" autostarty="true" loop="true" volumen="30" width="0" height="0">
  <ul class="posts noList">
    {% for post in paginator.posts %}
      <li>
        <span class="date">{{ post.date | date: '%B %d, %Y' }}</span>
        <h3><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p>{% if post.description %}{{ post.description }}{% else %}{{ post.excerpt | strip_html }}{% endif %}</p>
      </li>
    {% endfor %}
  </ul>
  <!-- Pagination links -->
  <div class="pagination">
    {% if paginator.previous_page %}
      <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}" class="previous button__outline">Temas nuevos</a> 
    {% endif %}
    {% if paginator.next_page %}
      <a href="{{ paginator.next_page_path | prepend: site.baseurl }}" class="next button__outline">Temas siguientes</a>
    {% endif %}
  </div>

