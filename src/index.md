---
layout: layouts/base
title: Welcome to Sassy Roots Apothecary
category: featured

card:
  - title: My Cool Product
    img: curry.jpg
    body: Catechin teacup strainer lychee teapot oolong london fair trade.
    #full-click: true
    buy: true
    price: "$10"
    url: "/"
    link:
      - text: my link
        url: "/"
    badge: "Special"
  - title: My Cool Product
    img: curry.jpg
    body: Catechin teacup strainer lychee teapot oolong london fair trade.
    #full-click: true
    buy: true
    price: "$10"
    url: "/"
  - title: My Cool Product
    img: curry.jpg
    body: Catechin teacup strainer lychee teapot oolong london fair trade.
    #full-click: true
    buy: true
    price: "$10"
    url: "/"
  - title: My Cool Product
    img: curry.jpg
    body: Catechin teacup strainer lychee teapot oolong london fair trade.
    #full-click: true
    buy: true
    price: "$10"
    url: "/"
---
<div class="home-hero">

![image of various root herbs on a wooden board is the background of this pages hero and sets the tone for the website](/assets/img/sassy-background.png)
# Welcome to Sassy Roots Apothecary
</div>


<div class="container md:grid md:grid-cols-2 md:gap-4">
  <div>

  ## Launched finally
  After over a decade of learning, it's time for me to finally share what I know with the world. This site is the hub space for my herbal practice served as a magazine style website with each issue being dedicated to a herb with stories, recipes, remedies, tutorials, and podcast. Most importantly, community building and education through our local meetups and our online community. 

  Stay tuned to the space for more... and...

  {% meetup %} | {% discord %}
  </div>
  <div class="md:border-l-2 md:p-10">

  ### Excuse the mess / Changelog
  This site is still under construction and far from the brand experience I plan to build.

  However...with version beta.2.. I now have full cart functionality allowing you to order products directly from the site... **YAY!** ... with both shipping options and local pick up. 
  </div>
</div>

<div class="home-shop">

## Now in store
{% assign shop = collections.featured %}
{% include "patterns/shop-3up.md" %}

<div style="margin: 15px;"><a  href="/shop">view all products <i class="fa-duotone fa-arrow-right"></i></a></div>
</div>

<div class="my-6 container">

## Consult with me
Consult with me for custom formulary that will help you with out your spiritual herbal goals. Find out more about how I can [assist](https://sassyroots.com/consultations/) and book an [appointment](https://sassyroots.com/consultations/).
</div>

