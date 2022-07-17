---
title: Lösryckta tankar
layout: page
permalink: blogg
---
{%- if site.posts.size > 0 -%}
    {%- for post in site.posts -%}
      {%- assign date_format = "%d%m%y" -%}
      [{{ post.date | date: date_format }}] <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></br>
    {%- endfor -%}
{%- endif -%}
