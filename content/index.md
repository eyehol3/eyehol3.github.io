---
layout: page
title: content
permalink: /questionable_content/
---
<h1> quality_content <sup>trademark</sup><br></h1>

  {% for post in site.posts %}
  {% if post.categories.last contains "content" %}
    
{% if post.starred %}<span class="starred">★</span>{% endif %}<a href="{{ post.url }}">{{ post.title }}</a> <span class="date">{{ post.date | date: "%d-%m-%Y"}}</span>

  {% endif %}
  {% endfor %}
