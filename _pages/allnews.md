---
title: "News"
layout: textlay
excerpt: "DAN Lab news"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{ article.date }} <br> {{ article.headline | markdownify | remove: '<p>' | remove: '</p>' }}
{% endfor %}
