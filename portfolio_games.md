---
layout: default
title: Games
navbar_name: Portfolio
stylesheet_name: page_project_list
permalink: /portfolio/games/
---
<!-- Games -->
<div class="title-container">
	<h1>Games</h1>
</div>

<div style="padding: 25px;"></div>

<div class="projects-list container marketing">
	{% assign games = site.games | sort: "release_date" | reverse %}
	{% for game in games %}
		{% include element_game_preview.html %}
	{% endfor %}
</div>
