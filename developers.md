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
	<h2>APIs</h2>
	<ul>
		<li>Nahezu vollständige Implementierung der pr0gramm-API: <a href="//github.com/holzmaster/OpenPr0gramm">OpenPr0gramm</a>, geschrieben in C# 6 mit Support für TAP (async/await)</li>
		<li>Java-API, die die <a href="//github.com/mopsalarm/Pr0">pr0gramm-Android-App</a> verwendet</li>
		<li>Bald: Node.js-API (noch in Entwicklung)</li>
	</ul>
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
