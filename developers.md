---
layout: page
title: Entwickler
permalink: /developers/
---
<section>
	Du bist Entwickler und willst etwas für das pr0gramm entwickeln?
	Hier findest to APIs, und Tools, die dir dabei helfen.
</section>
<section>
	Diese Pr0grammer haben bereits etwas für das pr0gramm entwickelt:
	<ul>
	{% for post in site.posts %}
		<li>{{ post.author }} von {{ post.title }}</li>
	{% endfor %}
	</ul>
</section>
