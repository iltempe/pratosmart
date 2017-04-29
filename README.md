# Pratosmart
Questo repository contiente tutti i post del progetto Pratosmart coordinato da Matteo Tempestini da Gennaio 2014 a Marzo 2016.

Tutti i post del progetto sono distribuiti con licenza di libero riuso Creative Commons CC BY 4.0,
il che significa che puoi usarli e riusarli per fare qualunque cosa tu voglia a patto di citare la loro provenienza.

Se vuoi maggiori informazioni su questa licenza consulta questa pagina
http://creativecommons.org/licenses/by/4.0/

<div class="panel-group">
{% for member in post %}
<div class="panel-body">
<a href="/issues/{{ member.number | datapage_url: '.' }}" class="list-group-item">
	<h4 class="list-group-item-heading">{{member.title}}</h4>
	<p class="list-group-item-text">{{member.issue.data.descrizione|markdownify}}</p>
	<p class="list-group-item-text">{{member.issue.data.data}}</p>
</a>
</div>
{% endfor %}
</div>
