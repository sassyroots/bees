<div class="card-group">
{% for c in card %}
{% if c.full-click %}
<div class="card full-click">
<a href="{{ c.url }}">
{% else %}
<div class="card">
{% endif %}
{% if c.img %}<img src="/assets/img/{{ c.img }}">{% endif %}
<div>
{% if c.title %}<h3>{{ c.title }}</h3>{% endif %}
{% if c.body %}
{{ c.body | markdownify }}
{% endif %}
{% if c.buy %}
<span class="buy"><i class="fa-duotone fa-cart-shopping"></i> ${{ c.price }} <a href="{{ c.url }}">Get Details</a></span>
{% elsif  c.link %}
{% for l in c.link %}
<a class="{{ l.class | default: "btn" }}" href="{{ l.url }}">{{ l.text }}</a>
{% endfor %}
{% endif %}
</div>
{% if c.badge %}
<div class="badge"><span>{{ c.badge }}</span></div>
{% endif %}
{% if c.full-click %}
</a>
{% endif %}
</div>
{% endfor %}
</div>