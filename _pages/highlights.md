---
title: "BAND Framework - Highlights"
layout: gridlay
excerpt: "BAND Framework -- Highlights."
sitemap: false
permalink: /highlights/
---


# Highlights (one pagers)

Jump to [physics highlights](#physics-highlights).

## Methodology Highlights


{% assign number_printed = 0 %}
{% for highlight in site.data.highlights %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if highlight.display == 1 and highlight.type == "methodology" %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ highlight.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/highlightpic/{{ highlight.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ highlight.description }}</p>
  <p><b>Contact: </b><em>{{ highlight.contact }}</em></p>
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}/highlights/{{ highlight.link.pdf }}" target="_blank">{{ highlight.link.text }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

Jump to [physics highlights](#physics-highlights).

## Physics Highlights


{% assign number_printed = 0 %}
{% for highlight in site.data.highlights %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if highlight.display == 1  and highlight.type == "physics" %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ highlight.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/highlightpic/{{ highlight.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ highlight.description }}</p>
  <p><b>Contact: </b><em>{{ highlight.contact }}</em></p>
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}/highlights/{{ highlight.link.pdf }}" target="_blank">{{ highlight.link.text }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

