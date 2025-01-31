---
title: "NSL Lab - Pooria"
layout: personal
permalink: /people/pooria-namyar/
sitemap: false
excerpt: "Personal website of Pooria"
---
{%- assign data = site.data.people -%}
{%- assign member = data.pooria -%}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="22%" style="float: left" />
  <h1>{{ member.name }}</h1>
  <i style="font-size:20px">{{ member.info }}</i><br>

  {% if member.website %}<a href="{{ member.website }}" target="_blank"><i class="fa fa-home fa-3x"></i></a> {% endif %}
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
  <!-- {% if member.cv %} <a href="{{ site.url }}{{ site.baseurl }}/files/{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %} -->
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  {% if member.linkedin %} <a href="{{ member.linkedin }}" target="_blank"><i class="fa fa-linkedin-square fa-3x"></i></a> {% endif %}
  {% if member.twitter %} <a href="{{ member.twitter }}" target="_blank"><i class="fa fa-twitter-square fa-3x"></i></a> {% endif %}
  <!-- {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %} -->
  <ul style="overflow: hidden">

  {% for education in member.education %}
	<li> {{ education }} </li>
  {% endfor %}

  </ul>
</div>

## Sketch

<p>I am a Ph.D. student in the <a href="https://minghsiehece.usc.edu/" data-type="URL" data-id="https://minghsiehece.usc.edu/">ECE department</a> at the <a href="https://www.usc.edu/">University of Southern California</a>. I am currently a member of <a href="https://nsl.usc.edu/">Networked Systems Lab</a> and very fortunate to be advised by <a href="https://govindan.usc.edu/">Prof. Ramesh Govindan</a>. Generally, I am interested in every aspect of computer networks and systems. My recent focus is on datacenter networks, wide-area networks, network availability, and reliability. </p>
<p>Before joining USC, I completed my B.Sc. in <a href="http://ee.sharif.edu/~web/en/">Electrical Engineering</a> at the <a href="http://www.en.sharif.edu/">Sharif University of Technology</a> in 2019.  During my undergraduate, I worked on the cloudification of telecommunication networks by leveraging SDN and NFV. </p>
<p>Feel free to drop me an email if you have any questions or want to discuss new ideas!</p>

## Work Experience

<p><em>Graduate Research Assistant</em> (Aug 2019 - present) <br>University of Southern California, Los Angeles, CA</p>
<p><em>Research Intern</em> (Jun 2022 - Jan 2023)<br>Microsoft Research, Redmond, WA<br>Mentors: <a href="https://www.microsoft.com/en-us/research/people/bearzani/">Behnaz Arzani</a>, <a href="https://www.microsoft.com/en-us/research/people/rybecket/">Ryan Beckett</a>, <a href="https://www.microsoft.com/en-us/research/people/srikanth/">Srikanth Kandula</a></p>
<p><em>Research Intern</em> (Jun 2021 - Jan 2022)<br>Microsoft Research, Redmond, WA<br>Mentors: <a href="https://www.microsoft.com/en-us/research/people/bearzani/">Behnaz Arzani</a>, <a href="https://www.microsoft.com/en-us/research/people/dacranks/">Dan Crankshaw</a>, <a href="https://www.microsoft.com/en-us/research/people/srikanth/">Srikanth Kandula</a></p>

{% if member.awards %}
## Awards
{% endif %}

{% for award in member.awards %}
<ul style="overflow: hidden">
<li> {{ award }} </li>
</ul>
{% endfor %}

## Publications

<div class="publications">

{% bibliography -f people/pooria%}

</div>
