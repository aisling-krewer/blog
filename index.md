---
layout: default
title: Home
---

# Welcome to My Blog

A collections of thoughts, ramblings and notes to try and reinforce what I've learned lately!

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

## Debug: All Posts
Post count: {{ site.posts.size }}

{% for post in site.posts %}
- Title: {{ post.title }}
- Date: {{ post.date }}
- File: {{ post.path }}
{% endfor %}