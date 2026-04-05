---
layout: page
title: Categories
permalink: /categories/
---

### Blog Categories

{% for category in site.categories %}
  #### {{ category | first }}
  <ul>
    {% for post in category.last %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date_to_string }}</li>
    {% endfor %}
  </ul>
{% endfor %}
