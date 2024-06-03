---
title: Components
layout: components
nav_order: 1
---

{% for component in site.components %}
  <h2>{{ component.title }} - {{  }}</h2>
  <p>{{ component.content | markdownify }}</p>
{% endfor %}
