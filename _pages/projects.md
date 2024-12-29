---
layout: page
title: 看看
permalink: /sumuzhe/
description:
nav: true
nav_order: 3
display_categories: ["电影", "剧集", "纪录片"]
---

{% assign projects_by_year = site.projects | group_by_exp: "project", "project.date | date: '%Y'" %}
{% assign sorted_year = projects_by_year | sort: "name" | reverse %}

<!-- pages/projects.md -->
<div class="projects">
  {% for year in sorted_year %}
    {% if year.name >= "2021" %}
      <div class="year">
        <a href="{{ year.name | prepend: '/sumuzhe/' | prepend: site.baseurl}}">
        <i class="fa-solid fa-calendar fa-sm"></i>
          {{ year.name }}
        </a>
      </div>
      <div class="review-stats">
        {% include review_stats.liquid projects=year.items cats=page.display_categories %}
      </div>
    {% endif %}
  {% endfor %}

  {% assign legacy_projects = site.projects | where_exp: "project", "project.date >= '2016-01-01' and project.date < '2021-01-01'" %}
    <div class="year">
      <a href="{{ '2016-2020' | prepend: '/sumuzhe/' | prepend: site.baseurl}}">
        <i class="fa-solid fa-calendar fa-sm"></i>
          2016 至 2020
      </a>
    </div>
    <div class="review-stats">
      {% include review_stats.liquid projects=legacy_projects cats=page.display_categories %}
    </div>

  {% assign legacy_projects = site.projects | where_exp: "project", "project.date < '2016-01-01'" %}
    <div class="year">
      <a href="{{ 'before2016' | prepend: '/sumuzhe/' | prepend: site.baseurl}}">
        <i class="fa-solid fa-calendar fa-sm"></i>
          更久以前
      </a>
    </div>
    <div class="review-stats">
      {% include review_stats.liquid projects=legacy_projects cats=page.display_categories %}
    </div>
</div>
