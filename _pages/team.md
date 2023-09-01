---
title: "Our Team"
excerpt: ""
author_profile: true
permalink: /team/
redirect_from: 
  - /about.html
---

 * <b><font color= "#737373" >ICT division Bangladesh research grant </font></b>(2020-2021): 1000K BDT
 * <b><font color= "#737373" >CUET IT business incubator research grant </font></b>(2019-2020): 400K BDT
 
# Team Members
(Please click the name below for the lab memeber's profile)

## Faculty
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="/images/labs/sarahpreum.jpg" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="https://persist-lab02.github.io/" class="off">Sarah Masud Preum</a></h4>
  <i> Director Persist-Lab</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
