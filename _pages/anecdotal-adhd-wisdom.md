---
layout: single
title: "ADHD Wisdom"
author_profile: true
permalink: /anecdotal-adhd-wisdom/
---
<em>Young people with ADHD are some of the funniest, most creative people I've ever met. They also have ways of observing themselves and their frustrations that cut straight to the bone. Here's some of their assorted wisdom that I've collected over the years.</em>

{% for page in site.wisdom %}
<div class="anecdote-card">

<span><p>{{page.content}}</p></span>
<span class='anecdote-tweet'></span>
<span class="anecdote-text">#add #adhd #adhd{{page.tags | join:" #"}}</span>
</div>
<br>
{% endfor %}