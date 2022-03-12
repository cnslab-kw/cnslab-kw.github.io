---
title: "News"
layout: textlay
excerpt: "CNS Lab at Kwangwoon University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}

{{ article.date }}
{{ article.headline | markdownify}}

{% endfor %}
