---
title: Overview
layout: components
nav_order: 1
---

Words
<div>
 <div style="display: grid; grid-template-columns: repeat(3, 1fr)">
  {% for component in site.components %}
  <div>
    <a href="{{site.baseurl}}{{ component.url }}">
      <h3>{{ component.title }}</h3>
      <p>{{ component.intro | markdownify }}</p>
    </a>
  </div>
  {% endfor %}  
 </div>
</div>
