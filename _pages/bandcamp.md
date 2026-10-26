---
title: "BAND Framework - BAND Camp"
layout: gridlay
excerpt: "BAND Framework -- BAND Camp."
sitemap: false
permalink: /bandcamp/
---

# BAND Camp


BAND has held four *BAND camps* to disseminate BAND tools and ideas to the community. 
One was completely virtual (December 2020), one hybrid (December 2021), and two in-person (May 2023 and October 2026). These were all in conjunction with workshops on Information and Statistics in Nuclear Experiment and Theory ([ISNET](https://isnet-series.github.io/meetings/)). 

----

Jump to 
* videos and slides from [BAND Camp 2023](#band-camp-2023)

----

## BAND Camp 2026 (October 5, 2026) 

BAND Camp 2026 was a one-day set of pedagogical presentations and tutorials organized by the Bayesian Analysis of Nuclear Dynamics (BAND) collaboration. Materials were geared towards students and earlier career researchers, and aimed to provide an introduction to the software tools developed by BAND and to the corresponding concepts and methods of Bayesian uncertainty quantification. 

The camp taught attendees to use Bayesian statistics, which is a mathematical method for updating the probability of a hypothesis as more evidence becomes available. In nuclear physics, researchers can use BAND tools when fitting (or "calibrating") a model to experimental data, when estimating the uncertainties in a particular model, and in order to combine disparate models of a particular observable. 

BAND’s software has tools that are designed to facilitate these steps in the Bayesian workflow. The software thus lowers the barrier for nuclear-physics researchers wishing to employ Bayesian methods, acting as a "bridge" between applied math and nuclear physics data.


{% for talk in site.data.presentations %}

{% if talk.type == "BAND_Camp_2026" %}

  <a href="{{talk.link.url }}" target="_blank"><em>{{ talk.title }}</em></a>
  {% if talk.video == 1 -%}   
  \[<a href="{{talk.video_link.url }}" target="_blank">video</a>\]
  {%- endif -%}  
  <br />
  {{ talk.presenter }} <br />{{ talk.location }}<br />{{ talk.date}}<br />

{% endif %}

{% endfor %}


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