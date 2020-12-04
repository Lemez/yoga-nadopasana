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
<li><a href="../assets/pdf/sarali-varisai-complete.pdf">Sarali Varisai</a></li>
<li><a href="../assets/pdf/jantai-varisai-complete.pdf">Jantai Varisai </a></li>
<li><a href="../assets/pdf/daatu-varisai-complete.pdf">Daatu Varisai </a></li>
<li><a href="../assets/pdf/melstaayi-varisai-complete.pdf">Melstaayi Varisai </a></li>
<li><a href="../assets/pdf/mandrastaayi-varisai-complete.pdf">Mandrastaayi Varisai </a></li>
</ol>
### Sheet Music {#geethams}
<ul>
    <li><a href="../assets/pdf/KamalaJadalaDocumentation.pdf">Kamala Jadala (Raga Kalyani)</a></li>
</ul>

### Online lectures {#lectures}
{% assign groups = site.lectures | group_by: "level" %}
{% for array in groups %}
{% assign arrays = array.items | group_by: "type" %}
{% for group in arrays %}
{% assign subgroups = group.items | group_by: "artist" %}
{% for subgroup in subgroups %}
{% assign idstring = group.name | capitalize | append: subgroup.name | slugify %}
<p id="idstring"><b>{{group.name | capitalize}} - {{subgroup.name }}</b></p> 
<ul>
{% for item in subgroup.items %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
{% endfor %}
{% endfor %}
{% endfor %}

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

## Watching {#watching}
<ul>
{% for item in site.watching %}
<li><a href="{{ item.video }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>

## Reading
### Jonathan's Blog {#blog}
Some blog posts from my time in India
{% assign pages = site.blog | sort: "title" %}
 <ul>
 {% for item in pages %}
<li><a href="{{ item.url }}"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
### Library {#library}
Articles and books for more in-depth research
<ul>
    {% for page in site.reading %}
    <li><a href="../assets/pdf/{{page.title}}.pdf">{{page.title}}, {{page.author}}</a></li>
    {% endfor %}    
</ul>
### Websites {#sites}
 <ul>
 {% for item in site.websites %}
<li><a href="{{ item.link }}" target="_blank"><b>{{ item.title }}</b></a><br>
{{item.description}}</li>
{% endfor %}
</ul>
