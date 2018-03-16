---
title: "SoftMatter Lab - Research"
layout: textlay
excerpt: "Soft Matter Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

We conduct experimental research on small scales with complex fluids. A big part of the research is devoted to gas and vapor bubbles, the deformation of biological cells, the response of biological material to acoustic waves, and fluid dynamics on the nanoscale.

Research of the SoftMatter Lab is mostly curiosity driven. Historically, I became interested in the peculiarities of bubbles from the phenomenon of [sonoluminescence](https://en.wikipedia.org/wiki/Sonoluminescence). In short it is the conversion of fluidic kinetic energy into visible light, aka photons. 

{% assign number_printed = 0 %}
{% for member in site.data.research_items %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if member.description %} <!-- only if some info available -->
<div class="col-sm-6 clearfix">
<div class="well">
<pubtit>{{ member.short }}</pubtit>
<p><img src="{{ site.url }}{{ site.baseurl }}/images/slider_home_edit/{{ member.name }}" class="img-responsive" style="border-radius:5%"/></p>
<p><em> {{ member.description }}</em></p>
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
