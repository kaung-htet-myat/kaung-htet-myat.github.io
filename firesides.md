---
layout: page
title: Firesides
permalink: /firesides/
---

{% for post in site.posts %}
  <div style="margin-bottom: 2em;">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p style="color: #666; font-size: 0.9em;">{{ post.date | date: "%B %d, %Y" }}</p>
  </div>
  <hr>
{% endfor %}
