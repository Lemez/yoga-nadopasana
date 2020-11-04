---
layout: single
title: "Getting Started"
author_profile: true
header:
    # text: Getting Started
    # image: /assets/images/trinity-colour-banner.jpg
    # caption: "The trinity of Carnatic composers"
    overlay_image: /assets/images/tanpura-banner.jpg
  # overlay_filter: rgba(205, 0, 0, 0.5)
permalink: /guide/
---
{% assign pages = site.guide | sort: "order" %}
<ol>
{% for page in pages %}
<li style="margin-top:1em;font-weight:400;"><a style="text-decoration: none;" href="{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ol>