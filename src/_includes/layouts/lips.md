---
layout: layouts/product
---
### ingredients
{% if herbs %}
  {{ prod.lipbalm.ingredients | join: ", " }}, with infused herbs - {{ herbs | join: ", " }}
{% endif %}

## ${{ prod.lipbalm.price | plus: upprice }}
<button class="snipcart-add-item"
  data-item-id="{{ sku }}"
  data-item-price="{{ prod.lipbalm.price | plus: upprice }}"
  data-item-weight="{{ prod.lipbalm.weight }}"
  data-item-url="http://sassyroot.netlify.app{{ url }}"
  data-item-description="{{ short }}"
  data-item-image="/img/prod/{{ img.thumb }}"
  data-item-name="{{ title }}"
  data-item-custom1-name="Flavors"
  data-item-custom1-options="{{ prod.lipbalm.vars }}"
  data-item-custom2-name="Size"
  data-item-custom2-options="{{ prod.lipbalm.pricing }}">
  Add to cart
</button>
