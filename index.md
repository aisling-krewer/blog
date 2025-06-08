---
layout: default
title: Welcome to My Blog!
---

## A collections of thoughts, ramblings and notes to try and reinforce what I've learned lately!

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}