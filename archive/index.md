---
layout: page
title: archive
permalink: /archive/
---
<h1 class="title"> The Archive </h1>
TRASH / personal-public notes / cringe / hidden gems / ахуєнні монологи / 
<br>
<br>

  {% for post in site.posts %}
  {% if post.categories.last contains "archive" %}

<!-- {%- if post.starred -%}<span class="starred">★</span>{%- endif -%} -->
<a href="{{ post.url }}">{{ post.title }}</a> <span class="date">{{ post.date | date: "%Y-%m-%d"}}</span>

  {% endif %}
  {% endfor %}
