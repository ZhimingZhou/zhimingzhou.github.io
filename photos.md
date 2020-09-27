---
layout: default
title: Photos
permalink: /Photos/
comment_issue_id: 1
---

 <div>
	{% for image in site.static_files %}
	    {% if image.path contains '/photos/shows/' %}  
	        <img src="{{image.path}}" alt="{{ image.name }}" />
	    {% endif %}  
	{% endfor %}
</div>