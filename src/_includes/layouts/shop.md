---
layout: layouts/base
---

# {{ title }}
- hero here

<div class="container grid grid-cols-4 gap-1">
  <div class="left-nav">
  category nav here
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