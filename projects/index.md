---
layout: page
title: Projects
show_in_menu: true
permalink: /projects/
---

These pages describe some of the projects I've done or taken part in.

{% assign pages = site.pages | sort: 'title' %}
{% for page in pages %} {% if page.category == 'project' %}
[{{ page.title }}]({{ page.url }}) — {{ page.description }}

{% endif %} {% endfor %}
