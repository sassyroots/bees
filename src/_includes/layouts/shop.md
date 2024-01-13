---
layout: layouts/base
---

# {{ title }}{: .container .my-6 }


<div class="container grid grid-cols-4 gap-1">
  <div class="left-nav">
    <ul>
      {% for sn in collections.prod-landing %}
      <li><a href="{{ sn.url }}">{{ sn.data.title}}</a></li>
      {% endfor %}
    </ul>
  </div>
  <div class="col-span-3">
  {{ content }}
  <div class="card-group">
  {% for p in collections[category] %}
  {% include "patterns/shop-card.md" %}
  {% endfor %}
  </div>
  </div>
</div>