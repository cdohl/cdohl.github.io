---
title: "Home"
layout: textlay
excerpt: "SoftMatter & Cavitation Lab"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<div class="col-sm-6 clearfix">
<p><strong>{{ article.date }}</strong></p>
<p><em>{{ article.headline }}</em></p>
</div>
<br>
{% endfor %}
