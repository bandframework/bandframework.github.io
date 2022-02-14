---
title: "BAND Framework - Presentations"
layout: gridlay
excerpt: "BAND Framework -- Presentations."
sitemap: false
permalink: /presentations/
---


# Presentations

Jump to talks about [BAND methodology](#band-methodology), [BAND physics applications](#band-physics-applications).


## About BAND

{% for talk in site.data.presentations %}

{% if talk.type == "band" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}


Jump to talks about [BAND](#about-band), [BAND physics applications](#band-physics-applications).


## BAND methodology



Jump to talks about [BAND](#about-band), [BAND methodology](#band-methodology).

## BAND physics applications

