---
title: Write ups
layout: page
permalink: /writeup
---

{% assign sorted = site.writeups | sort: "title" %}

{% for w in sorted %}
- [{{ w.title }}]({{ w.url | relative_url }})
{% endfor %}
