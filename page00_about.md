---
layout: page
title: About & Syllabus
description: 
img: stem_cell.jpg
caption: "National Institute of Neurological Disorders and Stroke/NIH"
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
Our first meeting will take place on **Monday, September 29th, 2025**: please arrive promptly at **9am** in the Hexagone buildin, Room Hexalab at the first floor. On Friday much will be provided by CENTURI and on Monday, we will have a welcoming coffee between 9h and 9h30 and a coffee break between 10h and 10h20.

Each day will have a schedule roughly of the form:
<table style="border-collapse: collapse; width: 100%;">
  <tr style="background-color:#f2f2f2;">
    <th style="width:130px; border:1px solid #ccc; padding:8px;">Time</th>
    <th style="border:1px solid #ccc; padding:8px;">Session</th>
  </tr>
  <tr style="background-color:#d9d9d9;">
    <td style="border:1px solid #ccc; padding:8px;"><b>9h00</b> - 12h30</td>
    <td style="border:1px solid #ccc; padding:8px;">Lectures from Rob</td>
  </tr>
  <tr style="background-color:#f2f2f2;">
    <td style="border:1px solid #ccc; padding:8px;">12h30 - 13h30</td>
    <td style="border:1px solid #ccc; padding:8px;">Lunch Break</td>
  </tr>
  <tr style="background-color:#d9d9d9;">
    <td style="border:1px solid #ccc; padding:8px;">13h30 - 16h30 (will end at 15h on Friday)</td>
    <td style="border:1px solid #ccc; padding:8px;">Lectures from Rob</td>
  </tr>
  <tr style="background-color:#f2f2f2;">
    <td style="border:1px solid #ccc; padding:8px;">16h45 - 18h30 (15h15 - 17h on Friday)</td>
    <td style="border:1px solid #ccc; padding:8px;">Computation sessions with Sara</td>
  </tr>
</table>
