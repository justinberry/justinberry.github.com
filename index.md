---
layout: page
title: Software and 한국어 공부
tagline: 소프트웨어 재미있다!
---
{% include JB/setup %}

<h1>Posts</h1>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

