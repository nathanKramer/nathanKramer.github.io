---
layout: page
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
  * {{ post.date | date: date_format }} - [{{ post.title | escape }}]({{ post.url | relative_url }})
{% endfor %}
