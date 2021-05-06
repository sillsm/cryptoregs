---
layout: default
title: Chapter 2 SEC
chapter: SEC
---
st


{% for slice in site.chapter2_sec_howey %}
{% for h1 in slice.sections %}
    <p>
    <a href="{{ slice.url | relative_url }}#{{ h1 }}">
     {{ h1 }}
    </a>
    </p>
    
    {% for h2 in h1 %}
    <p>
    <a href="{{ slice.url | relative_url }}#{{ h2 }}">
    {{ h2 }}
    </a>
    </p>
    
    {% endfor %}

{% endfor %}
{% unless slice.sections % }
 <p>{{ slice.title }}</p>
{% endunless % }
{% endfor %}


{% for slice in site.chapter2_sec_howey %}
 {{ slice.content }}
{% endfor %}
