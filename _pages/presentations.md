---
title: "BAND Framework - Presentations"
layout: gridlay
excerpt: "BAND Framework -- Presentations."
sitemap: false
permalink: /presentations/
---


# Presentations

----

Jump to talks about [BAND methodology](#band-methodology) or [BAND physics applications](#band-physics-applications).

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


