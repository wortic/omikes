---
title: Lösryckta tankar
layout: page
permalink: blogg
---
{%- if site.posts.size > 0 -%}
  <ul id="different" style="list-style-type: none">
    {%- for post in site.posts -%}
    <li>
      {%- assign date_format = "%d%m%y" -%}
      [{{ post.date | date: date_format }}] <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </li>
    {%- endfor -%}
  </ul>
{%- endif -%}
