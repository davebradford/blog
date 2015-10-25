---
layout: default
title: Writing
permalink: /blog/
---

{% for post in site.posts %}
<div class="grid_12 omega">
  <h2>{{ post.title }}</h2>
  <p>{{ post.excerpt }}</p>
  <button><a href="{{ post.url }}">Read More</a></button>
</div>
{% endfor %}