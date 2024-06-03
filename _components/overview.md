---
title: Overview
layout: components
nav_order: 1
---

{% for component in site.components %}
    <a href="{{site.url}}{{component.url}}">
      <div>
          <img class=""  style="" height="auto" width="100%" alt="">
      </div>
      <div>
          <h2 class="" style="">{{component.title}}</h2>
      </div>
      <div>
          <span>An avatar is a visual representation of a user or entity.
      </div>
    </a>
{% endfor %}
