<div class="foot">
<div class="foot-container">
  <div class="footbar">
    <div class="foot-logo">
      {% logo "light" %}
    </div>
    <div class="foot-nav nav-sm">
      <ul>
      {% for item in nav.foot %}
      {% unless item.state == "draft" %}
        <li><a href="{{ item.url }}">{{ item.title }}</a></li>
      {% endunless %}
      {% endfor %}
      </ul>
    </div>
    <div class="foot-copy">
     <p class="notice">Notice: No federal agency regulates herbalists. As such, all articles, recipes, and products do not claim to heal, treat, or cure diseases, as these terms are strictly used by licensed doctors. Rather, the information contained here is simply advice gathered from herbalists and indigenous healers here in the United States, and medical practitioners in Asia, Africa, and the Caribbean who still follow the plant ways of our ancestral heritages. Occasionally, information is sourced from the National Institutes of Health (NIH), which is beginning to study and believe in such wisdom.<br/> <br/> Being educated and caring for your body is both your right and responsibility, regardless of whether you are seeking advice from an herbalist, an alternative healer, a spiritualist, or a medical professional. Taking care of yourself is the most revolutionary and sassiest thing you can do.</p>
     <p>&copy 2023 Sassy Roots Apothecary. All rights reserved.</p>
    </div>
  </div>
  <div class="foot-nav nav-md">
      <ul>
      {% for item in nav.foot %}
      {% unless item.state == "draft" %}
        <li><a href="{{ item.url }}">{{ item.title }}</a></li>
      {% endunless %}
      {% endfor %}
      </ul>
    </div>
</div>
</div>