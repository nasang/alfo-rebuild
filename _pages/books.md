---
layout: page
title: 读读
permalink: /zizijin/
description:
nav: true
nav_order: 4
---

{% assign books_by_year = site.books | group_by_exp: "book", "book.date | date: '%Y'" %}
{% assign sorted_year = books_by_year | sort: "name" | reverse %}

<div class="books">
    {% for year in sorted_year %}
        <h2 class="year">{{ year.name }}</h2>
        {% assign books = year.items %}
        <div class="container">
            <div class="row">
            {% for book in books %}
                {% include books.liquid book=book %}
            {% endfor %}
        </div>
    {% endfor %}
</div>
