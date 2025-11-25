---
layout: page
title: "Study Notes"
permalink: /study/
---

# Study Notes

공부한 내용을 정리한 글들입니다.

{% for post in site.posts %}
  {% if post.categories contains "study" %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
  {% endif %}
{% endfor %}