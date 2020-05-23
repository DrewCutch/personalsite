---
title: All Posts
layout: default
---

# All Posts:
{% for post in site.posts %}
<h3>
    <a href="{{ post.url }}">{{ post.title }}</a>
     - 
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
</h3>
{% endfor %}