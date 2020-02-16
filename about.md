---
layout: default
title: Temas propuestos
---
  <h1 class="pageTitle">Temas Propuestos</h1>
  <embed src="{{ '/assets/img/' | prepend: site.baseurl }}" autostarty="true" loop="true" volumen="30" width="0" height="0">
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
 <font color="#32CC32"><h2><center>¿Por qué consideramos estos temas?:<br></center></h2></font>
 <p class="intro" aling="justify"><span class="dropcap">S</span>Se selecionaron estos temas por motivos de bla bla bla</p>  
<h4>Dele click para ver el tema</h4><br>
 <h4><a href="https://blogdelenguaje.github.io/blog/ViciosdelLenguaje/">-Vicios del Lenguaje</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/EstructuradelParrafo/">-Estructura del Parrafo</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/NormasOrtografica/">-Normas Ortográficas.</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/RedacciondeuntextoAcademico/">-La redacción de un texto Académico</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/tema5/">-Tema 5</a><br></h4> 
  <h4><a href="https://blogdelenguaje.github.io/blog/tema6/">-Tema 6</a><br></h4>


