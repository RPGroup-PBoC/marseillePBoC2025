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
Our first meeting will take place on **Monday, September 29th, 2025**: please arrive promptly at **9am** in the Hexagone buildin, Room Hexalab at the first floor. On Friday much will be provided by CENTURI and on Monday, we will have a welcoming coffee between 9h and 9h30 and a coffee break between 10h and 10h20.

Each day will have a schedule roughly of the form:
<table>
<tr>
    <th style="width:130px"><b>Time</b></th>
    <th><b>Session</b></th>
</tr>
<tr>
    <td><b>9h00</b> - 12h30</td>
    <td>Lectures from Rob</td>
</tr>
<tr>
    <td>12h30 - 13h30</td>
    <td>Lunch Break</td>
</tr>
<tr>
    <td>13h30 - 16h30 (will end at 15h on Friday)</td>
    <td>Lectures from Rob</td>
</tr>
<tr>
    <td>16h45 - 18h30 (15h15 - 17h on Friday)</td>
    <td>Computation sessions with Sara</td>
</tr>
</table>