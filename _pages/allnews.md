---
title: "Plasma Photonics Team - News"
layout: textlay
excerpt: "P2 Team @ GoLP -- Research"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline | markdownify}}</p>
{% endfor %}
