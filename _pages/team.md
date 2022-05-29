---
title: "CNS Lab - Team"
layout: gridlay
excerpt: "CNS Lab: Team members"
sitemap: false
permalink: /team/
---

# Members

<!-- **We are looking for new Master/Undergraduate students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/openings) **!**-->


{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.link %}
  <h3>[{{ member.name }}]({{site.url}}/{{member.link}})</h3>
  {% else %}
  <h3>{{ member.name }}</h3>
  {% endif %}
  <i>{{ member.info }}</i><br>
  <b>Email:</b> {{ member.email }}
  {% if member.research %}<br><b>Research Interests:</b> {{ member.research }} {% endif %} 

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


