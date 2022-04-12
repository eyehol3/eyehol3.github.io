---
layout: page
title: journal
permalink: /journal/
---
# my journal and other notes idk
<br>
blablabla
<br>

  {% for post in site.posts %}
  {% if post.categories.last contains "journal" %}

{% if post.starred %}<span class="starred">★</span>{% endif %}<a href="{{ post.url }}">{{ post.title }}</a> <span class="date">{{ post.date | date: "%d-%m-%Y"}}</span>

  {% endif %}
  {% endfor %}
