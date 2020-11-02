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
---
## Online Groups
We currently practice every Sunday at 1100 CET online. There is no cost. If you would like to join us, we would be grateful if you could [tell us a bit about yourself](https://forms.gle/yT6gxFSK8bt232JAA) first.

## What Students Say
{% assign pages = site.testimonials | sort: "location" %}
{% for page in pages %}
<div style="display:block;">
<p>{{page.content}}</p>
<p style="float:right;"><em>{{page.type}} ({{ page.location }})</em></p>
</div>

<br>
<hr>
{% endfor %}