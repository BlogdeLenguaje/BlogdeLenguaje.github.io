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
 <p class="intro" aling="justify"><span class="dropcap">E</span> El tema de este Blog es “Lineamientos y Sugerencias para el buen uso de la Lengua Escrita” con dicho tema quisimos dar un poco de ayuda a aquellos estudiantes o personas que se están adentrando en el aprendizaje de la lengua española, ya que los subtemas que hemos propuesto conllevan a reforzar la utilización de las reglas ortográficas. Esto lo hemos tomado en cuenta debido al bajo conocimiento y manejo de la lengua escrita, dentro del ámbito académico, en un gran porcentaje de los estudiantes universitarios. Así, dado estas ayudas básicas, el alumno podrá guiarse y realizar una redaccion decente y aprenderá a manejar lineamientos preestablecidos a la hora de escribir un texto. Espero que los temas aquí expuestos sean de mucha ayuda a los visitantes de este blog.
  X</p>  
<h4>Dele click para ver el tema</h4><br>
 <h4><a href="https://blogdelenguaje.github.io/blog/ViciosdelLenguaje/">-Vicios del Lenguaje</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/EstructuradelParrafo/">-Estructura del Parrafo</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/NormasOrtografica/">-Normas Ortográficas.</a><br></h4>
  <h4><a href="https://blogdelenguaje.github.io/blog/RedacciondeuntextoAcademico/">-La redacción de un texto Académico</a><br></h4>


