---
title: Posts
permalink: /Posts/
layout: default
---

{%- if site.posts.size > 0 -%}
  
  <ul class="post-list">
    {%- for post in site.posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ post.date | date: date_format }}
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h3>
      </li>
    {%- endfor -%}
  </ul>
  
{%- endif -%}