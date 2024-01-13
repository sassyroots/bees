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


</div>

<div class="bg-gray-300">
<div class="container mt-20 py-10">

## You may also like
{% include "patterns/shop-3up.md" %}
</div>
</div>
