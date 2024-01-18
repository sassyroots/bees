---
layout: layouts/product
---
### ingredients
{% if herbs %}
  {{ herbs | join: ", " }}
{% endif %}

## starts at ${{ prod.tea.price | plus: upprice }}
<button class="snipcart-add-item btn"
  data-item-id="{{ sku }}"
  data-item-price="{{ prod.tea.price | plus: upprice }}"
  data-item-weight="{{ prod.tea.weight }}"
  data-item-url="{{ settings.site_url }}{{ prod.tea.url}}{{ url }}"
  data-item-description="{{ short }}"
  data-item-image="/assets/img/shop/{{ img.thumb }}"
  data-item-name="{{ title }}"
  data-item-custom2-name="Sizes"
  data-item-custom2-options="{{ prod.tea.vars }}">
  Add to cart
</button>
