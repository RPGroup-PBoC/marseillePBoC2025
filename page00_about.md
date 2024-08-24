---
layout: page
title: About & Syllabus
description: 
img: darwinPlantCircumnutation.svg
caption: "after C. Darwin, 1896"
permalink: index.html
sidebar: true
---

# {{site.data.about.title}}
{{site.data.about.authors}}

{% for entry in site.data.about %}

{% if entry[0] != 'title' %}
{% if entry[0] != 'authors' %}
## {{entry[0]}}
{{entry[1]}}
{% endif %}
{% endif %}
{% endfor %}

# Syllabus
<table>
<tr>
    <th><b>Day</b></th>
    <th><b>Date</b></th>
    <th><b>Topic</b></th>
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.day}}</td>
    <td>{{day.date}}</td>
    <td>{{day.topic}}</td>
</tr>
{% endfor %}
</table>

# When and Where