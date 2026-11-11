---
layout: page
title: experience
permalink: /projects/
description:
nav: true
nav_order: 3
display_categories: [research]
horizontal: true
---

<style>
  /* Keep the research cards text-only, consistently bordered in the theme purple. */
  .projects .research-card-grid .card.hoverable {
    border: 1px solid var(--global-theme-color);
  }

  .projects .research-card-grid .card.hoverable .card-title {
    font-size: 1.1rem;
    font-weight: 700;
  }

  .projects .research-card-grid .card.hoverable .row > [class*="col-md-6"]:first-child {
    display: none;
  }

  .projects .research-card-grid .card.hoverable .row > [class*="col-md-6"]:last-child {
    flex: 0 0 100%;
    max-width: 100%;
  }
</style>

<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
    {% for category in page.display_categories %}
      <h2 class="category" id="{{ category }}" style="text-align: left;">{{ category }}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <div class="container research-card-grid">
        <div class="row row-cols-1 row-cols-md-2">
          {% for project in sorted_projects %}
            {% include projects_horizontal.liquid %}
          {% endfor %}
        </div>
      </div>
    {% endfor %}
  {% else %}
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <h2 class="category" style="text-align: left;">research</h2>
    <div class="container research-card-grid">
      <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.liquid %}
        {% endfor %}
      </div>
    </div>
  {% endif %}

  <h2 class="category" id="service" style="text-align: left;">service</h2>
  <div class="container">
    <div class="row row-cols-1 row-cols-md-3">
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <a href="https://www.blackeudaimonia.org/" aria-label="Black Eudaimonia website" style="display: block; height: 100%;">
            <img src="{{ '/assets/img/be-logo.png' | relative_url }}" alt="Black Eudaimonia logo" style="width: 100%; height: 100%; padding: 16px; object-fit: contain;">
          </a>
        </div>
      </div>
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <a href="https://chapel.howard.edu/huasb" aria-label="Howard University Alternative Spring Break website" style="display: block; height: 100%;">
            <img src="{{ '/assets/img/huasb-logo.png' | relative_url }}" alt="HU Alternative Spring Break logo" style="width: 100%; height: 100%; padding: 16px; object-fit: contain;">
          </a>
        </div>
      </div>
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <a href="https://jumpstartkids.org/" aria-label="Jumpstart website" style="display: block; height: 100%;">
            <img src="{{ '/assets/img/jstart-logo.png' | relative_url }}" alt="Jumpstart College Corps logo" style="width: 100%; height: 100%; padding: 16px; object-fit: contain;">
          </a>
        </div>
      </div>
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <a href="https://booleangirl.org/" aria-label="Boolean Girl website" style="display: block; height: 100%;">
            <img src="{{ '/assets/img/booleangirl-logo.jpeg' | relative_url }}" alt="Boolean Girl logo" style="width: 100%; height: 100%; padding: 16px; object-fit: contain;">
          </a>
        </div>
      </div>
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <img src="{{ '/assets/img/bam-logo.png' | relative_url }}" alt="National Capital Area Blacks at Microsoft Academy logo" style="width: 100%; height: 220px; padding: 16px; object-fit: contain;">
        </div>
      </div>
      <div class="col mb-4">
        <div class="card" style="height: 220px;">
          <a href="https://brownkidsread.org/" aria-label="Brown Kids Read website" style="display: block; height: 100%;">
            <img src="{{ '/assets/img/bkr-logo.png' | relative_url }}" alt="Brown Kids Read logo" style="width: 100%; height: 100%; padding: 16px; object-fit: contain;">
          </a>
        </div>
      </div>
    </div>
  </div>
</div>
