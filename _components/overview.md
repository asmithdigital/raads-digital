---
title: Overview
layout: components
nav_order: 1
---

{% for component in site.components %}
    <a href="{{site.url}}/{{ component.url }}">
      <div style="padding: 24px">
        <div class="" style="">
          <img class=""  style="" height="auto" width="100%" alt="">
          <div class="" style="">
            <h2 class="" style="">{{ component.title }}</h2>
          </div>
          <span class="" style="">An avatar is a visual representation of a user or entity.</span></div>
      </div>
    </a>
{% endfor %}
