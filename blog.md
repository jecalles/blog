---
layout: default
title: blog
description: what I write when I'm not working
permalink: /blog/
---

{% for post in site.posts %}
  <div class="blog-item">
    <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
    <p class="meta"><i>{{ post.description }}</i></p>
    <p class="meta">{{ post.date | date_to_string }}</p>
  </div>
{% endfor %}
