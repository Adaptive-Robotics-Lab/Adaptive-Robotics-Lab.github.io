---
layout: page
title: Gallery
permalink: /gallery/
description: Moments from the Adaptive Robotics Lab.
nav: true
nav_order: 5

gallery:
  - image: IMG_1901.jpg
    alt: Lab members by the Chicago lakefront
  - image: IMG_2078.jpg
    alt: Lab members sharing a meal
  - image: IMG_5133.jpg
    alt: Adaptive Robotics Lab group outing
  - image: IMG_6498.jpg
    alt: Lab members at Korean barbecue
  - image: IMG_7386.jpg
    alt: Lab dinner gathering around hot pot
---

<div class="lab-gallery" aria-label="Adaptive Robotics Lab photo gallery">
  {% for photo in page.gallery %}
    {% capture photo_path %}/assets/img/Gallery/{{ photo.image }}{% endcapture %}
    {% include figure.liquid path=photo_path alt=photo.alt class="lab-gallery-image" zoomable=true sizes="(max-width: 575px) 95vw, 440px" %}
  {% endfor %}
</div>
