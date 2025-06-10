---
layout: page
title: Fireside Chats
permalink: /firesides/
---

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: "%b %-d, %Y" }}</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

