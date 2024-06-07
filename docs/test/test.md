---
title: Test
layout: home
has_children: true
---
all pages
{% for item in site.pages %}
{% if item.parent == "Test" %}
  These shoes are awesome!
{% endif %}
{% endfor %}
