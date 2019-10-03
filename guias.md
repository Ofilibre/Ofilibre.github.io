---
layout: archive
permalink: /guias/
title: "Guías de la OfiLibre"
image:
  feature: logo-ofilibre-blanco.jpg
---

{{ title }}

<div class="tiles">
{% for guia in site.guias %}
  {% assign coll = site.collections | where: "label", "guias" | first %}
  {% assign dir = guia.url | split: "/" | last | replace: '.html', '' %}
	{% include guia-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

