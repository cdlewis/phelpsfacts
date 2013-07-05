---
layout: page
title: Peter Phelps Facts
---
{% include JB/setup %}

{% assign counter = 0 %}
{% for post in site.posts %}
{% capture counter %}{{ counter | plus: '1' }}{% endcapture %}
<h2>{{ counter }}</h2>
{{ post.content }}
{% endfor %}