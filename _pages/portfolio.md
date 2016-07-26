---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: false
gallery:
  - url: codewars.png
    image_path: github.png
    alt: "placeholder image 1"
  - url: github.png
    image_path: learning.jpg
    alt: "placeholder image 2"

---

{% include base_path %}

<div class="grid__wrapper">
  {% for post in site.portfolio %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
