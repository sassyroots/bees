<div class="card">
  <img src="/assets/img/shop/{{ p.data.img.thumb }}">
  <div class="card-body">
  <h3> {{ p.data.title }} </h3>
  <p>{{ p.data.short | markdownify }}</p>
  <p class="buy"><i class="fa-duotone fa-cart-shopping"></i> <a href="{{ p.url }}">Get Details</a></p>
  {% if p.data.badge %}
  <div class="badge"><span>{{ p.data.badge }}</span></div>
  {% endif %}
  </div>
</div>