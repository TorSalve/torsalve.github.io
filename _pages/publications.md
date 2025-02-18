---
title:
layout: default
permalink: /publications/
published: true
---

Highlighted publications
====



<div class="PublicationContainer">

	<div class="gallery">


  {% for publication in site.publications %}

  <div class="publicationTile">
    {% if publication.redirect %}
      <a href="{{ publication.redirect }}" target="_blank">
    {% else %}
      <a href="{{ publication.url | prepend: site.baseurl | prepend: site.url }}">
    {% endif %}
      <div class="content">
        <div class="title">
          {% if publication.image %}
          <img class="publication-image" src="{{ publication.image | prepend: '/assets/images/publications/' | prepend: site.baseurl | prepend: site.url }}">
          {% endif %}
          <h3>{{ publication.title }}</h3>
        </div>
        <div class="description">
          <p><i>{{ publication.year }}</i></p>
          <p>{{ publication.description }}</p>
        </div>
      </div>
    </a>
  </div>

  

  {% endfor %}

	</div>

</div>

Publications
====

{% bibliography %}

