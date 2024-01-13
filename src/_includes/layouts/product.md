---
layout: layouts/base
---

<article class="container product" markdown="1">

![{{ img.alt }}](/assets/img/shop/{{ img.photo[0] }})

<div class="prod-details">

# {{ title }}
{{ short}}

{{ content }}
</div>
</article>

<div class="container">

{% if dosage %}
### how to use
{{ dosage }}
{% endif %}

{% if notice %}
### notice
{{ notice }}
{% endif %}


## You may also like
{% include "patterns/shop-3up.md" %}

</div>