---
title: "Soft Matter Lab - Publications"
layout: gridlay
excerpt: "Soft Matter Lab -- Publications."
sitemap: false
permalink: /publications/
---
# Publications

(For a full list see below or go to [Google Scholar](https://scholar.google.de/citations?user=g8LFI-EAAAAJ), [Researchgate](https://www.researchgate.net/profile/Claus_Dieter_Ohl?ev=hdr_xprf))

{% nolinebreaks %}
{% for i in (2001..2018) reversed %}
<a href="#linkyear{{ i }}"> {{ i }} |</a> 
{% endfor %}
{% endnolinebreaks %}

{% for i in (2001..2018) reversed %}
<p><a name="linkyear{{ i }}"> {{ i }}</a></p>
{% bibliography --query @*[year={{ i }}] %}
{% endfor %}
<p> Before 2001 </p>
{% bibliography --query @*[year<=2000] %}

