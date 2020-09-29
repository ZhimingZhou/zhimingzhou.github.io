---
title: Photos
permalink: /Photos/
layout: default
---

<div>
	{% for image in site.static_files %}
	    {% if image.path contains '/photos/shows/' %}  
	        <img src="{{image.path}}" alt="{{ image.name }}" />
	    {% endif %}  
	{% endfor %}
</div>