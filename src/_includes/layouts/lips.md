---
layout: layouts/product
---
### ingredients
{% if herbs %}
  {{ prod.lipbalm.ingredients | join: ", " }}, with infused herbs - {{ herbs | join: ", " }}
{% endif %}

## ${{ prod.lipbalm.price | plus: upprice }}
<button class="btn snipcart-add-item"
  data-item-id="{{ sku }}"
  data-item-price="{{ prod.lipbalm.price | plus: upprice }}"
  data-item-weight="{{ prod.lipbalm.weight }}"
  data-item-length="{{ prod.lipbalm.length }}"
  data-item-height="{{ prod.lipbalm.height }}"
  data-item-width="{{ prod.lipbalm.width }}"
  data-item-url="{{ settings.site_url }}{{ prod.lipbalm.url}}{{ url }}"
  data-item-description="{{ short }}"
  data-item-image="/img/prod/{{ img.thumb }}"
  data-item-name="{{ title }}"
  data-item-custom1-name="Flavors"
  data-item-custom1-options="{{ prod.lipbalm.vars }}">
  <i class="fa-duotone fa-cart-plus"></i> Add to cart
</button>
