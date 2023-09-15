---
layout: page
title: Readings
img: reading.png 
permalink: readings
caption: "DNA Sequence Chromatogram"
sidebar: true
---

---

<!--
This page autogenerates a list of readings by day and a collated list of links. 
All information is scraped from the _data/readings.yaml and _data/links.yaml.
Edit those to update the website
-->


{% for day in site.data.readings %}
## {{day[0]}}
{% for pub in day[1] %}
* <a href="{{site.baseurl}}/assets/pdfs/{{pub.link}}" target="_blank">**{{pub.title}}** by
  <i>{{pub.authors}}</i> ({{pub.year}})</a> {%if pub.description
  %}{{pub.description}}{%endif%}
{%endfor%}
{%endfor%}

<center>
<h1> Useful links</h1>
</center>

---

{%for link in site.data.links%}
* <a href="{{link.address}}" target="_blank">**{{link.title}}**</a> {%if link.description %}{{link.description}}{%endif%}
{%endfor%}

