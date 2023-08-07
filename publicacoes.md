---
layout: single
title: Publicações
permalink: /publicacoes/
---

<ul>
{% for publication in site.data.publicacoes %}
	<li>
		<b>Título</b>: {{ publication.title }} <br>
		<b>Autores</b>: {{ publication.authors }} <br>
		<b>Revista</b> ou evento: {{ publication.where }} <br>
		<b>Data de Publicação</b>: {{ publication.data }} <br>
		<b>DOI</b>: {{ publication.doi }}
	</li>
{% endfor %}
</ul>