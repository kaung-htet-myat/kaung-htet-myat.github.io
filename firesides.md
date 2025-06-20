---
layout: page
title: ""
permalink: /firesides/
---

{% if site.posts.size == 0 %}
  <h3>Fireside blogs coming soon...</h3>
{% else %}
{% for post in site.posts %}
  <div style="margin-bottom: 2em;">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p style="color: #666; font-size: 0.9em;">{{ post.date | date: "%B %d, %Y" }}</p>
    {% if post.excerpt %}
      {{ post.excerpt }}
    {% endif %}
  </div>
  <hr>
{% endfor %}
{% endif %}