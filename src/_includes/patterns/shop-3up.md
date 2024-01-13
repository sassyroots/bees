
<div class="card-group">
{% for p in collections[category] limit: 3 %}
{% unless title == p.data.title %}
{% include "patterns/shop-card.md" %}
{% endunless %}
{% endfor %}
</div>