---
title: "Plasma Photonics Team - News"
layout: textlay
excerpt: "P2 Team @ GoLP -- Research"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{ article.date }} <br> <strong> {{ article.headline}} </strong> <br> {{ article.fullstory | markdownify | remove: '<p>' | remove: '</p>' }}

{% if article.number_photo == 1 %}
     <img src="{{ site.url }}{{ site.baseurl }}/images/newspic/{{ article.photo }}" class="img-responsive" width="50%" style="display: block; margin: 0;" />
     {{ article.photo_caption }}
{% endif %}
{% endfor %}


