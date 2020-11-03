---
layout: single
title: "Practice With Us"
author_profile: true
header:
    # image: /assets/images/jon-with-border-1-sm.JPG
    # caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
    overlay_image: /assets/images/IMG_3777-banner.JPG
   # caption: "Embodied Voicework from South India"
  # overlay_filter: rgba(205, 0, 0, 0.5)
permalink: /testimonials/
toc: true
gallery:
  - url: /assets/images/IMG_3767.JPG
    image_path: /assets/images/IMG_3767.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
  - url: /assets/images/IMG_3777.JPG
    image_path: /assets/images/IMG_3777.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
  - url: /assets/images/IMG_3789.JPG
    image_path: /assets/images/IMG_3789.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
  - url: /assets/images/IMG_3835.JPG
    image_path: /assets/images/IMG_3835.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
  - url: /assets/images/IMG_3780.JPG
    image_path: /assets/images/IMG_3780.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
  - url: /assets/images/IMG_3823.JPG
    image_path: /assets/images/IMG_3823.JPG
    title: "ISHT Integral Sound Healing Training course, Svaram, 2018"
---
## Online Groups
We currently practice every Sunday at 1100 CET online. There is no cost. If you would like to join us, we would be grateful if you could [tell us a bit about yourself](https://forms.gle/yT6gxFSK8bt232JAA) first.

## Student Reactions

{% include video id="PWKARWORUmY" provider="youtube" %}

{% assign pages = site.testimonials | sort: "location" %}
{% for page in pages %}
{% if forloop.index==4 %}
{% include video id="CJHVWDwD-Ww" provider="youtube" %}
{% endif %}

<div style="display:block;">
<p>{{page.content}}</p>
<p style="float:right;"><em>{{page.type}} ({{ page.location }})</em></p>
</div>

<br>
<hr>

{% endfor %}

## Gallery
{% include gallery  %}