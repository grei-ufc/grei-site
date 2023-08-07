---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
author_profile: true
title: Pesquisadores
permalink: /pesquisadores/
---

<!-- <div class="entries-{{ entries_layout }}">
  <ul>
  {% for pesquisador in site.data.pesquisadores %}
      <li>
        <b> {{ pesquisador.name }} </b> <br>
        Posição: {{ pesquisador.position }} <br>
        Currículo Lattes: {{ pesquisador.lattes }}
      </li>
  {% endfor %}
  </ul>
</div> -->

<div class="entries-{{ entries_layout }}">
  <ul>
  {% for pesquisador in site.pesquisadores %}
      <li>
        <a href="{{ pesquisador.url }}"> {{ pesquisador.name }} </a> <br>
        Posição: {{ pesquisador.position }} <br>
        Currículo Lattes: {{ pesquisador.lattes }}
      </li>
  {% endfor %}
  </ul>
</div>


{% include paginator.html %}
