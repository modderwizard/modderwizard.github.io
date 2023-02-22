---
layout: default
title: Websites
navbar_name: Portfolio
stylesheet_name: page_project_list
permalink: /portfolio/websites/
---
<!-- Websites -->
<div class="title-container">
	<h1>Websites</h1>
</div>

<div style="padding: 25px;"></div>

<div class="projects-list container marketing">
	{% assign websites = site.websites | sort: "release_date" | reverse %}
	{% for website in websites %}
		{% include element_website_preview.html %}
	{% endfor %}
</div>