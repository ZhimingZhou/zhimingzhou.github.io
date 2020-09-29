---
title: Posts
permalink: /Posts/
layout: default
---

{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}

{%- if site.posts.size > 0 -%}
  
  <ul class="post-list">
    {%- for post in site.posts -%}
		{%- if post.top == true and hide != true -%}
			<li>
				{{ post.date | date: date_format }}
				<h3>
					[STICKY] <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
				</h3>
			</li>
		{%- endif -%}
    {%- endfor -%}
  </ul>
  
{%- endif -%}

{%- if site.posts.size > 0 -%}
  
  <ul class="post-list">
    {%- for post in site.posts -%}
		{%- if post.top != true and post.hide != true -%}
			<li>
				{{ post.date | date: date_format }}
				<h3>
					<a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
				</h3>
			</li>
		{%- endif -%}
    {%- endfor -%}
  </ul>
  
{%- endif -%}