---
layout: page
title: 看看
permalink: /sumuzhe/
description:
nav: true
nav_order: 3
display_categories: ["电影", "剧集"]
---

{% assign projects_by_year = site.projects | group_by_exp: "project", "project.date | date: '%Y'" %}
{% assign sorted_year = projects_by_year | sort: "name" | reverse %}

<!-- pages/projects.md -->
<div class="projects">
  {% for year in sorted_year %}
  <div class="year">
    <a href="{{ year.name | prepend: '/sumuzhe/' | prepend: site.baseurl}}">
    <i class="fa-solid fa-calendar fa-sm"></i>
      {{ year.name }}
    </a>
  </div>
  <div class="review-stats">
  {% include review_stats.liquid projects=year.items cats=page.display_categories %}
  </div>
  {% endfor %}
</div>
