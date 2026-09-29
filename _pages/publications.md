---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---

{% capture publication_count %}{% bibliography_count --file publications %}{% endcapture %}
{% assign publication_count = publication_count | plus: 0 %}

<div class="publications publications-list">
  {% if publication_count > 0 %}
    {% bibliography --file publications %}
  {% else %}
    <p class="publications-empty">Publication details will be added here.</p>
  {% endif %}
</div>
