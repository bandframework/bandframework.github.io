---
title: "BAND Framework - Software"
layout: gridlay
excerpt: "BAND Framework: Software"
sitemap: false
permalink: /software/
---

# Software 

External code delivery will be from the [bandframework github repository](https://github.com/bandframework/bandframework)


{% assign number_printed = 0 %}
{% for sw in site.data.softwarelist %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
   <code style = "font-size-adjust: 1.1; color:black; justify-content: center;"> {{ sw.name }} </code>
   <img src="{{ sw.imageurl }}" class="img-responsive" width="25%" style="float: left;padding: 10px 10px 10px 10px;" />
   <p>{{ sw.info }}</p>
   <em>{{ sw.authors }} </em><br /><a href="{{ sw.link.url }}">{{ sw.link.display }}</a>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

# Software Development Kit


<hr>
