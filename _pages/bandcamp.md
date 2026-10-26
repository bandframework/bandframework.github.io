---
title: "BAND Framework - BAND Camp"
layout: gridlay
excerpt: "BAND Framework -- BAND Camp."
sitemap: false
permalink: /bandcamp/
---

# BAND Camp

BAND has held four *BAND camps* to disseminate BAND tools and ideas to the community. 
One was completely virtual (December 2020), one hybrid (December 2021), and two in-person (May 2023 and October 2026). These were all in conjunction with workshops on Information and Statistics in Nuclear Experiment and Theory (ISNET). 


----

Jump to 
* videos and slides from [BAND Camp 2023](#band-camp-2023)
----

## BAND Camp 2026

----

## BAND Camp 2023


{% for talk in site.data.presentations %}

{% if talk.type == "BAND_Camp_2023" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a>
  {% if talk.video == 1 -%}   
  \[<a href="{{talk.video_link.url }}" target="_blank">video</a>\]
  {%- endif -%}  
  <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}<br />

{% endif %}

{% endfor %}

----

## Second Annual BAND Camp (2021)

----

## First Annual BAND Camp (2020)