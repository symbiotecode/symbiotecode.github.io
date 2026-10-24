---
layout: default
title: Blog Posts
---

# Welcome to my Blog

Here is a list of my latest articles:

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
*Published on {{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}
{% endfor %}

