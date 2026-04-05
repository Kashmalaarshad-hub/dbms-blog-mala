---
layout: page
title: My Lab Blog
permalink: /blog/
---

{% for post in site.posts %}
  ### [{{ post.title }}]({{ post.url | relative_url }})
  *Published on: {{ post.date | date_to_string }}*
  
  {{ post.excerpt | strip_html | truncatewords: 30 }}
  [Read More...]({{ post.url | relative_url }})
  ---
{% endfor %}
