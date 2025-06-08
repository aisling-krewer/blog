---
layout: default
title: Home
---

# Welcome to My Blog

This is my GitHub Pages project site built with Jekyll!

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}