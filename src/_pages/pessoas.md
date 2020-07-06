---
layout: hero
title: "Equipe"
permalink: /equipe/
---

<div class="row align-items-center pt-2 pt-lg-5">
    <div class="col-md-7">
        <h2>Equipe</h2>
        <p class="lead">O PRACTICE conta com uma equipe de estudantes e professores que se dedicam de forma organizada e eficiente para realizar diversos tipos de atividades.</p>
    </div>
    <div class="col-md-1"></div>
    <div class="col-md-4">
        <p><img alt="image" class="img-fluid" src="https://cdn.jsdelivr.net/gh/froala/design-blocks@2.0.1/dist/imgs/draws/tabs.svg"></p>
    </div>
</div>

<section class="fdb-block">
  <div class="container">
    <div class="card-group">
      {% assign people = site.data.people | sort:"name" %}
      {% for person in people %}
        {% include person-grid.html %}
      {% endfor %}
    </div>
  </div>
</section>