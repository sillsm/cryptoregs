---
layout: default
title: Chapter 2 SEC
chapter: SEC
---
step

{% include toc.html html=content sanitize=true class="inline_toc" id="my_toc" h_min=1 h_max=3 %}

{% for slice in site.chapter2_sec_howey %}
{% assign content = slice.content  %}
 {{ content }}
{% endfor %}
