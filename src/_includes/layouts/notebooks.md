---
layout: layouts/product
---
Paper Prints: ${{ prod.notebooks.price | plus: upprice }} | PDF Download ${{ prod.notebooksdl.price | plus: upprice }}
<div class="">
<button class=" btn snipcart-add-item"
  data-item-id="{{ sku }}"
  data-item-price="{{ prod.notebooks.price |plus: upprice }}"
  data-item-description="{{ short }}"
  data-item-image="/img/prod/{{ img.thumb }}"
  data-item-url="{{ settings.site_url }}{{ prod.notebooks.url}}{{ url }}"
  data-item-name="{{ title }}"
  data-item-file-weight="{{ prod.notebooks.weight }}">
  <i class="fa-duotone fa-cart-plus"></i> Buy paper book
</button>


<button class=" btn snipcart-add-item"
  data-item-id="{{ sku }}-pdf"
  data-item-price="{{ prod.notebooksdl.price |plus: upprice }}"
  data-item-description="{{ short }}"
  data-item-image="/assets/img/prod/{{ img.thumb }}"
  data-item-url="{{ settings.site_url }}{{ prod.notebooks.url}}{{ url }}"
  data-item-name="{{ title }} PDF"
  data-item-file-guid="{{ guid }}">
  <i class="fa-duotone fa-download"></i> Buy PDF
</button>
</div>
