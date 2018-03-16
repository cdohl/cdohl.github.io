---
title: "SoftMatter Lab - Team"
layout: gridlay
excerpt: "SoftMatter Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni).

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}
  
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
 
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  
  </ul>
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




## Master and Bachelor Students 
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}
  
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  
  </ul>
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



## Alumni
<img src="{{ site.url }}{{ site.baseurl }}/images/group2014.jpg" class="img-responsive" width="50%" style="float: center" />

{::nomarkdown}
<div class="container-fluid">
  <div class="row">
    <div class="col-sm-4">
      <strong> Former PostDocs and Staff</strong>
        <ul>
        <li>Asst Prof Manish Arora</li>
        <li>Asst Prof Pedro Quinto-Su</li>
        <li>Asst Prof Chen Longquan</li>
        <li>Asst Prof Keita Ando</li>
        <li>Asst Prof Hari Krishnan Unni</li>
        <li>Asst Prof Dr Santosh Raavi</li>
        <li>Dr Song Chaolong</li>
        <li>Dr Yang Yuanxing</li>
        <li>Dr Huang Xiaohu</li>
        <li>MSc Han Mengtong</li>
        <li>MSc Shripad Kulkarni</li>
        </ul>
    </div>
    <div class="col-sm-4">
      <strong> Former PhD and Master students</strong>
      <ul>
        <li>Dr Manish Arora</li>
        <li>Dr Rory Dijkink</li>
        <li>Dr Zhao Xue</li>
        <li>Dr Firdaus Prabowo</li>
        <li>Dr Chon U Chan</li>
        <li>Dr Fenfang Li</li>
        <li>Dr Tan Beng Hau</li>
        <li>Dr Meera Mohan</li>
        <li>Dr Luong Trung Dung</li>
        <li>Dr Milad Mohammadzadeh</li>
        <li>Dr Weiwei Chan</li>
        <li>MSc Anne Charlotte van Bloekland</li>
        <li>MSc Raghunath Venkatramanan</li>
      </ul>
    </div>
  </div>
</div>
{:/nomarkdown}