---
title: "Faculty"
layout: faculty
excerpt: "About me"
permalink: /jinwoo
---

# Faculty

<div class="row">
<div class="col-sm-3">
<img src="./images/teampic/jinwoo.jpg" class="img-responsive" width="80%">
</div>

<div class="col-sm-8">
### **Jinwoo Kim (김진우)**
* Assistant Professor at School of Software in Kwangwoon University
* <i class="fa-solid fa-envelope"></i> Email: jinwookim (at) kw.ac.kr
* <i class="fa-solid fa-phone"></i> Phone: +82-2-940-5185
* <i class="fa-solid fa-building"></i> Office: 807 Saebit Hall (새빛관 807호)
* <i class="fa-solid fa-building-columns"></i> [Google Scholar](https://scholar.google.com/citations?user=xou0CrcAAAAJ&hl=ko) 
* <i class="fa-brands fa-linkedin"></i> [LinkedIn](https://www.linkedin.com/in/jinwoo-kim-49a045164/)
</div>
</div>

--------------

<div class="col">
### <i class="fa-solid fa-user"></i> Short Bio
I am currently an assistant professor of School of Software at [Kwangwoon University](https://www.kw.ac.kr/en/index.jsp) since March 2022. Before joining here, I obtained my Ph.D. in School of Electrical Engineering and master degree in Graduate School of Information Security from [KAIST](https://www.kaist.ac.kr/en/) (Advisor: [Prof. Seungwon Shin](http://nss.kaist.ac.kr/?page_id=29)). I received my B.S from [Chungnam National University](https://plus.cnu.ac.kr/html/en/). My research interests broadly include cloud and network systems security, Software-Defined Networking (SDN), Network Function Virtualization (NFV), eBPF/XDP, and programmable data-plane.
</div>

--------------

### <i class="fa-solid fa-graduation-cap"></i> Education

* **Ph.D. in Electricial Engineering**
    + Korea Advanced Institute of Science and Technology (KAIST), Daejeon, Republic of Korea
    + Dissertation: Securing Software-Defined WAN Through Analyzing Network Attack Surfaces
    + Advisor: [Seungwon Shin](https://nss.kaist.ac.kr/?page_id=29)

* **Master in Information Security**
    + Korea Advanced Institute of Science and Technology (KAIST), Daejeon, Republic of Korea
    + Advisor: [Seungwon Shin](https://nss.kaist.ac.kr/?page_id=29)

* **B.S. in Computer Science and Engineering**
    + Chungnam National University, Daejeon, Republic of Korea

--------------
### <i class="fa-solid fa-book"></i> Publication

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

### <i class="fa-solid fa-chalkboard-user"></i> Talk

{% for publi in site.data.talklist %}

  {% if publi.url %}
  <b>{{ publi.title }}</b> <a href="{{ publi.url }}">(link)</a><br />
  {{ publi.authors }} <br />{{ publi.venue }}

  {% else %}
  <b>{{ publi.title }}</b> <em>(to appear)</em> <br />
  {{ publi.authors }} <br />{{ publi.venue }}
  {% endif %}

{% endfor %}

------------------

### <i class="fa-solid fa-user-tie"></i> Experience

<b>Resaerch Observer</b> (Supervisor: Phillip Porras)<br />
SRI International, Meonlo Park, CA, Summer 2019<br />

<b>Resaerch Observer</b> (Supervisor: Phillip Porras)<br />
SRI International, Meonlo Park, CA, Winter 2017<br />

------------------

### <i class="fa-solid fa-award"></i> Award

<b>The 28th Samsung Humantech Paper Award</b><br />
Silver Prize, Feburary 2022

<b>The 26th Samsung Humantech Paper Award</b><br />
Silver Prize, Feburary 2020


<script src="https://kit.fontawesome.com/392aa12767.js" crossorigin="anonymous"></script>
