---
title: "News"
layout: textlay
excerpt: "Laboratory for Molecular Modeling & Drug Discovery "
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
