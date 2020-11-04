---
layout: single
title: "Helpful Resources"
author_profile: true
header:
    image: /assets/images/quote-960.jpg
permalink: /resources/
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
### Sheet Music {#geethams}
<ul>
    <li><a href="../assets/pdf/KamalaJadalaDocumentation.pdf">Kamala Jadala (Raga Kalyani)</a></li>
</ul>

## Listening {#listening}
### Vocal {#listening-vocal}
{% assign vocal = site.listening | where: "type","vocal" %}
{% assign instrumental = site.listening | where: "type","instrumental" %}
<ul>
{% for item in vocal %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
### Instrumental {#listening-instrumental}
<ul>
{% for item in instrumental %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>


## Watch {#watching}
{% assign groups = site.watching | group_by: "level" %}
{% for array in groups %}
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

## Library {#library}
<ul>
    {% for page in site.reading %}
    <li><a href="../assets/pdf/{{page.title}}.pdf">{{page.title}}, {{page.author}}</a></li>
    {% endfor %}    
</ul>
## Blog {#blog}
{% assign pages = site.blog | sort: "title" %}
 <ul>
 {% for item in pages %}
<li><a href="{{ item.url }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
