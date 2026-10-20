---
layout: default
nav_order: 1
nav_title: Home
---

# A place to keep track of my crafting projects and other thoughts.

## Latest posts

{% for post in site.posts limit:5 %}
<p><strong><a href="{{ post.url | relative_url }}">{{ post.title }}</a></strong><br>
<small>{{ post.date | date: "%b %-d, %Y" }}</small></p>
<p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
{% endfor %}
