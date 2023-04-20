---
layout: page
title: Syllabus
img: reading.png 
permalink: syllabus
caption: "DNA Sequence Chromatogram"
sidebar: true
---


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