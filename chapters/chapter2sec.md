---
layout: default
title: Chapter 2 SEC
chapter: SEC
---
Some words here

* Table of Contents
{:toc}

{% for slice in site.chapter2_sec_howey %}
 <p>{{ slice.title }}</p>
{% endfor %}

{% for slice in site.chapter2_sec_howey %}
 {{ slice.content }}
{% endfor %}
