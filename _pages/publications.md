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
  {% if publication.published %}
  {% assign has_page = publication.content | strip | size %}
  {% if publication.doi %}{% capture paper_url %}https://doi.org/{{ publication.doi }}{% endcapture %}{% else %}{% assign paper_url = publication.redirect %}{% endif %}
  {% if has_page != "0" %}{% assign main_url = publication.url | prepend: site.baseurl %}{% else %}{% assign main_url = paper_url %}{% endif %}

  <article class="publicationTile">
    {% if publication.image %}
    <a class="publication-thumb" href="{{ main_url }}" tabindex="-1" aria-hidden="true">
      <img class="publication-image" src="{{ publication.image | prepend: '/assets/images/publications/' | prepend: site.baseurl }}" alt="">
    </a>
    {% endif %}
    <div class="publication-body">
      <h3><a href="{{ main_url }}">{{ publication.title }}</a></h3>
      <p class="publication-meta">
        {% if publication.publication %}{{ publication.publication }} &middot; {% endif %}{{ publication.year }}
      </p>
      <p class="publication-teaser">{{ publication.teaser | default: publication.description }}</p>
      <p class="publication-links">
        {% if has_page != "0" %}<a href="{{ main_url }}">Read the summary &rarr;</a>{% endif %}
        {% if paper_url %}<a href="{{ paper_url }}" target="_blank" rel="noopener">Paper</a>{% endif %}
      </p>
    </div>
  </article>

  {% endif %}
  {% endfor %}
  </div>
</div>

Publications
====

{% bibliography %}

