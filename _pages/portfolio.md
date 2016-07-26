---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: true
gallery:
  - url: sage.png
    image_path: sage.png
    alt: "placeholder image 1"
  - url: chatwebsite.png
    image_path: chatwebsite.png
    alt: "placeholder image 2"
  - url: dropbox.png
    image_path: dropbox.png
    alt: "placeholder image 3"

---

### Website Projects


{% include base_path %}
{% include gallery caption="" %}
<div class="grid__wrapper">
  {% for post in site.portfolio %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
