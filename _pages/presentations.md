---
title: "BAND Framework - Presentations"
layout: gridlay
excerpt: "BAND Framework -- Presentations."
sitemap: false
permalink: /presentations/
---


# Presentations

----

Jump to talks about [BAND methodology](#methodology-talks) or [BAND physics applications](#physics-talks).

<div id="band-talks">
----
</div>

## About BAND

{% for talk in site.data.presentations %}

{% if talk.type == "band" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}

----

Jump to talks about [BAND](#band-talks) or [BAND physics applications](#physics-talks).

<div id="methodology-talks">
----
</div>


## BAND methodology


{% for talk in site.data.presentations %}

{% if talk.type == "methodology" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}


----

Jump to talks about [BAND](#band-talks) or [BAND methodology](#methodology-talks).

<div id="physics-talks">
----
</div>

## BAND physics applications

{% for talk in site.data.presentations %}

{% if talk.type == "physics" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a> <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}

{% endif %}

{% endfor %}


