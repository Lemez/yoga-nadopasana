---
layout: single
title: "Hacks"
author_profile: true
permalink: /hacks-for-add-adhd/
---
{% assign types = site.techniques | group_by: "type"  %}
{% for type in types %}
<h2 class="titleize">{{type.name}} Hacks</h2>
{% assign ordered = type.items | sort: "order" %}
{% for item in ordered %}
<h3><a href="{{ item.link }}" target="_blank">{{ item.title }}</a></h3>
{{item.description}}
{% endfor %}
{% endfor %}
