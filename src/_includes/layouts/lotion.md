---
layout: layouts/product
---
{% assign pd = prod.lotion %}
### ingredients
{% if herbs %}
  {{ pd.ingredients | join: ", " }}, with infused herbs - {{ herbs | join: ", " }}
{% endif %}

## ${{ pd.price | plus: upprice }}
<button class="btn snipcart-add-item"
  data-item-id="{{ sku }}"
  data-item-price="{{ pd.price | plus: upprice }}"
  data-item-weight="{{ pd.weight }}"
  data-item-url="{{ settings.site_url }}{{ pd.url}}{{ url }}"
  data-item-description="{{ short }}"
  data-item-image="/assets/img/shop/{{ img.thumb }}"
  data-item-name="{{ title }}">
  <i class="fa-duotone fa-cart-plus"></i> Add to cart
</button>
