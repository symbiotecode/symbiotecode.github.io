---
layout: default
title: Blog Posts
---

# Welcome to my Blog

Let's connect on Bluesky 🦋!

---

### Latest Articles

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
*📅 {{ post.date | date: "%b %d, %Y" }} • ⏳ {{ post.content | strip_html | number_of_words | divided_by: 180 | plus: 1 }} min read*

{{ post.excerpt | strip_html | truncatewords: 30 }}  
[Read Article →]({{ post.url | relative_url }})

---
{% endfor %}


