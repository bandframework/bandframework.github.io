---
title: "BAND Framework - Presentations"
layout: gridlay
excerpt: "BAND Framework -- Presentations."
sitemap: false
permalink: /presentations/
---


# Presentations

----

Jump to 
* talks about [BAND](#about-band) or [BAND methodology](#band-methodology) or [BAND physics applications](#band-physics-applications).
* videos and slides from [BAND Camp 2023](#band-camp-2023)

----

## About BAND

{% for talk in site.data.presentations %}

{% if talk.type == "band" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}

----

Jump to talks about [BAND](#about-band) or [BAND physics applications](#band-physics-applications).

----

## BAND methodology

See also videos and slides from [BAND Camp 2023](#BAND-Camp-2023).

{% for talk in site.data.presentations %}

{% if talk.type == "methodology" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}


----

Jump to talks about [BAND](#about-band) or [BAND methodology](#band-methodology).

----

## BAND physics applications

{% for talk in site.data.presentations %}

{% if talk.type == "physics" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}


----

Jump to talks about [BAND](#about-band) or [BAND methodology](#band-methodology).

----

## BAND Camp 2023


{% for talk in site.data.presentations %}

{% if talk.type == "BAND_Camp_2023" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a>
  {% if talk.video == 1 %}   
  \[<a href="{{talk.video_link.url }}" target="_blank">video</a>\]
  {% endif %}  
  <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}<br />

{% endif %}

{% endfor %}

