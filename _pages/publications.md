---
title: "CNS Lab - Publications"
layout: gridlay
excerpt: "CNS Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

## International Conferences/Journals

{% for publi in site.data.publist %}

  {% if publi.url %}
  <b>{{ publi.title }}</b> <a href="{{ site.url }}{{ publi.url }}">(paper)</a><br />
  {{ publi.authors }} <br />{{ publi.venue }}

  {% else %}
  <b>{{ publi.title }}</b> <em>(to appear)</em> <br />
  {{ publi.authors }} <br />{{ publi.venue }}
  {% endif %}

{% endfor %}

-----------------

## Talk

{% for publi in site.data.talklist %}

  {% if publi.url %}
  <b>{{ publi.title }}</b> <a href="{{ publi.url }}">(link)</a><br />
  {{ publi.authors }} <br />{{ publi.venue }}

  {% else %}
  <b>{{ publi.title }}</b> <em>(to appear)</em> <br />
  {{ publi.authors }} <br />{{ publi.venue }}
  {% endif %}

{% endfor %}
