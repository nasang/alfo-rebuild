---
layout: page
title: 看看
permalink: /sumuzhe/
description: 
nav: true
nav_order: 3
horizontal: true
display_categories: # ["电影", "剧集"]
toc:
  sidebar: right
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "date" | reverse %}

  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    {% assign projects_by_year = sorted_projects | group_by_exp: "project", "project.date | date: '%Y'" %}
    {% for year in projects_by_year %}
    <h3>{{ year.name }} 年度统计</h3>
    <div class="row row-cols-1 row-cols-md-1">
      {% for project in year.items %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
    {% endfor %}
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "date" | reverse %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}
  <div class="container">
    {% assign projects_by_year = sorted_projects | group_by_exp: "project", "project.date | date: '%Y'" %}
    {% for year in projects_by_year %}
      <a id="{{ year.name }}" href=".#{{ year.name }}">
        <h2 class="category">{{ year.name }}</h2>
      </a>
      <div class="row row-cols-1 row-cols-md-1">
      {% for project in year.items %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
      </div>
    {% endfor %}
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
