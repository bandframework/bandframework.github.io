---
title: "BAND Framework - Presentations"
layout: gridlay
excerpt: "BAND Framework -- Presentations."
sitemap: false
permalink: /presentations/
---


# Presentations

## Invited Talks

{% for talk in site.data.presentations %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endfor %}
