---
layout: single
title:  "Finding Your Shruti"
type: 
order: 1
toc: true
---
### Finding your shruti
Although Nadopasana is a personal practice that we mostly do by ourselves, the sound that we produce is never alone, as we are always accompanied by a drone instrument, most typically a South Indian tanpura or a North Indian shruti box.

Your pitch (<em>shruti</em>) is the root note, the SA, which is your constant companion as you sing. I like to think of it as the ground that our voice will soar above and dive below, the unchanging point of reference which creates flow, tension and release in the music. 

Unlike Western music, the shruti of Indian music is always determined by the singer, so it is important to choose a shruti in which you are most comfortable. The easiest way to tell is that you should be able to sing one octave comfortably, going up from the root note of the drone.

{% include video id="pzz7NRhOv8Y?t=89" provider="youtube" %}

### Group Sessions / Individual Practice
You'll hear three strings in the tanpura recording, two octaves playing the root SA (in this case, A) and also the 5th note PA (in this case, E). 

For group practices, we usually use a shruti in A, which is good for most students. In group sessions we all use the same shruti, so go ahead and click on <b>Tanpura in A</b> below.

In case the shruti of A feels too low or too high for individual practice, I have uploaded other shrutis for you to sing with and see if you prefer. If none of these feel comfortable, please let me know and I will help you to find one that works.
<ul>
{% assign drones = site.tanpura | sort: "order" %}
{% for d in drones %}
{% unless d.semitone=="true" %}
<li><a href="{{d.video}}" target="_blank">{{d.title}}</a></li>
{% endunless %}
{% endfor %}
</ul>
### A Note on Your Shruti and Your Voice
You will notice as you sing that on some days your voice is naturally higher, and on others, naturally lower. This also depends on the time of day that you sing. 

When we sing in the morning, we are actually taller, and our muscles are longer, including our vocal cords. This means that slightly altering your shruti down by half a tone in the morning can make for an easier practice session. So if you usually use:
<ul>
{% for d in drones %}
{% if d.semitone=="true" %}
<li>{{d.related}}, try <a href="{{d.video}}" target="_blank">{{d.title}}</a></li>
{% endif %}
{% endfor %}
</ul>

### Buying An Instrument
Beginners usually use recordings, but if you do get deep into your practice and would like to get a real instrument, it does add an extra dimension to feel the vibrations physically in the room with you.

{% include video id="yYU-R8LSIfs" provider="youtube" caption="Although a stringed tanpura is traditional in South Indian music, as a trumpet player, I connect strongly to the bellows of a Hindustani shruti box and the feeling that I have some musical lungs singing beside me."%}

The best tanpuras are from Thanjavur in Tamil Nadu, and the best shruti boxes from Kolkata in Bengal. If you are considering getting an instrument, recommend speaking to one of the few shops/importers who know the tradition deeply. [This workshop from the Netherlands](https://www.tosslevy.nl/tanpura/) has a lot of detailed information about the history of the tanpura and sometimes instruments for sale. There are similarly [small importers/workshops](http://www.keshav-music.com/shruti-boxes) in the US . 

Please note, these are not personal recommendations. I bought my own instrument in Auroville, India, from my friends at the wonderful sound research and practice centre, [Svaram](http://www.svaram.org).



