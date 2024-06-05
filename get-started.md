---
layout: components
title: Get started
nav_order: 1
intro: How to get started with Apiary
---

test

{% assign subpage = [site.foundations, site.components, site.forms] | where: 'title', 'Overview' %}
{% for item in subpage %}
<div>
  <div class="category-tiles">
    <div>
      <a href="{{site.baseurl}}{{ item.url }}" class="{{item.title}}">
        {% if item.promo-image %}
          <div class="category-tiles-thumb"><img src="{{site.url}}assets/images/{{item.promo-image}}"></div>
        {% else %}
         <div class="category-tiles-thumb"></div>
        {% endif %}
        <h3>{{ item.category_title }}</h3>
        <p>{{ item.intro | markdownify }}</p>
      </a>
    </div>
  </div>
</div>
{% endfor %}
