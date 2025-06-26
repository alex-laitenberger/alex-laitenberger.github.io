---
layout: default
title: "Blog"
---

# Blog

{% for post in site.posts %}
  <article style="margin-bottom: 2em;">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
