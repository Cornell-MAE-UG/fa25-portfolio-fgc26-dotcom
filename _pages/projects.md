---
layout: default
title: Flavia Capet - Portfolio
permalink: /projects/
---

<h2 style="text-align: center;">MAE2250: ODP Project</h2>

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      {% if project.category == "odp" %}
        <div class="gallery-item">
          <a href="{{ project.url | relative_url }}">
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
            <p>{{ project.title }}</p>
          </a>
        </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

<h2 style="text-align: center;">Other Projects</h2>

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      {% unless project.category == "odp" %}
        <div class="gallery-item">
          <a href="{{ project.url | relative_url }}">
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
            <p>{{ project.title }}</p>
          </a>
        </div>
      {% endunless %}
    {% endfor %}
  </div>
</div>