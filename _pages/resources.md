---
layout: single
title: "Helpful Resources"
author_profile: true
permalink: /helpful-resources/
toc: true
---
## Practice {#practice}
### Tanpura {#tanpura}
<ul>
 {% for item in site.tanpura %}
<li><a href="{{ item.video }}" target="_blank">{{ item.title }}</a></li>
{% endfor %}
</ul>
### Exercises {#exercises}
<ol>
<li><a href="../assets/pdf/carnatic-ganamrutha-bodhini-lesson-1.pdf">Sarali Varisai A</a></li>
<li><a href="../assets/pdf/carnatic-ganamrutha-bodhini-lesson-1-c.pdf">Sarali Varisai B</a></li>
<li><a href="../assets/pdf/carnatic-ganamrutha-bodhini-lesson-2.pdf">Jantai Varisai A</a></li>
</ol>

## Listening {#listening}
### Vocal
{% assign vocal = site.listening | where: "type","vocal" %}
{% assign instrumental = site.listening | where: "type","instrumental" %}
<ul>
{% for item in vocal %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
### Instrumental
<ul>
{% for item in instrumental %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>


## Study {#reading}
{% assign groups = site.watching | group_by: "level" %}
{% for array in groups %}
### {{array.name}} {#{{array.name}}}
{% assign arrays = array.items | group_by: "type" %}
{% for group in arrays %}
{% assign subgroups = group.items | group_by: "artist" %}
{% for subgroup in subgroups %}
{% assign idstring = group.name | capitalize | append: subgroup.name | slugify %}
<h5 id="idstring">{{group.name | capitalize}} - {{subgroup.name }}</h5> 
<ul>
{% for item in subgroup.items %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
{% endfor %}
{% endfor %}
{% endfor %}
## Blog {#blog}
{% assign pages = site.blog | sort: "title" %}
 {% for item in pages %}

### [{{ item.title }}]({{item.url}})
{{item.description}}
{% endfor %}
