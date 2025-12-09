---
title: Write ups
layout: page
permalink: /writeup
---

Count: {{ site.writeups | size }}

{% assign sorted = site.writeups | sort: "title" %}

{% for w in sorted %}
- [{{ w.title }}]({{ w.url | relative_url }})
{% endfor %}
