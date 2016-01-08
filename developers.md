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
		<li>{{ post.title }} von {% if post.author %}
				{% for auth in post.author %}
					<a class="author" href="{{ auth | prepend: "/user/" | prepend: site.pr0gramm_url }}">{{ auth }}</a>
						{% if forloop.rindex0 > 0 %} und {% endif %}
				{% endfor %}
		{% endif %}</li>
	{% endfor %}
	</ul>
</section>
