<div class="head">
<div class="head-container">
  <div class="logo" alt="Sassy Roots Apothecary logo and link to home page"><a href="/">{% logo "light" %}</div>
  <div class="topnav" id="myTopnav">
    {% for item in nav.nav %}
    {% unless item.state == "draft" %}
      <a href="{{ item.href}}"
      {% if page.url == item.href %}
        class="active"
      {% endif %}
      > {{ item.title }}</a>
    {% endunless %}
    {% endfor %}
  </div>
  <div class="shopcart"><button class="snipcart-checkout">
    <span class="fa-layers fa-fw" style="font-size: 30px;">
    <i class="fa-duotone fa-cart-shopping text-white"></i>
    <span class="fa-layers-counter bg-accent" style="font-size: 50px; "><span class="snipcart-items-count"></span></span>
    </span>
    </button></div>
  
</div>
</div>