---
title: Lösryckta tankar
layout: page
---
<a href="javascript:history.back()">Bakåt</a>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date }}{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
