---
layout: default
title: Writings
---

# Writings

Here I share my poems, reflections, and occasional essays.

{% for post in site.pages %}
  {% if post.path contains 'writings/' and post.name != 'index.md' %}
  - [{{ post.title }}]({{ post.url | relative_url }})
  {% endif %}
{% endfor %}
