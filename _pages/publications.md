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

  <b>{{ publi.title }} </b> 

  {%- if publi.url -%}
  <a href="{{ site.url }}{{ publi.url }}">(paper)</a><br />
  {% else %}
  <em>(to appear)</em> <br />
  {%- endif -%}

  {% assign authors = publi.authors | split: ", " %}
  {%- for author in authors -%} 
  	{%- if author contains "Jinwoo Kim" -%}<em><b>{{author}}</b></em>
  	{%- else -%}{{ author }}
  	{%- endif -%}
	{% unless forloop.last %}, {% endunless %}
  {%- endfor -%}
  
  <br>
  {{ publi.venue }}
  {% if publi.rate %} (Acceptance rate: {{ publi.rate }}) {% endif %}

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
