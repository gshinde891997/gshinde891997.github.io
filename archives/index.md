---
layout: default
title: Archives
---

<h1>All Posts</h1>

<ul>
{% for post in site.posts %}
  <li>
    {{ post.date | date: "%Y-%m-%d" }} —
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
