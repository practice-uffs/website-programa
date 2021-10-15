---
layout: hero
title: "Recursos"
image:
  feature: banner-rotulo.png
permalink: /recursos/
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-md-7">
        <h1><b>Recursos</b></h1>
        <h2>Criamos conteúdos para aprimorar seus conhecimentos e facilitar sua vida</h2>
        <p class="lead mt-4">Precisa realizar uma videoconferência e não sabe qual a melhor forma de fazer? Precisa fazer um vídeo, animação ou imagem e tem dificuldade em lidar com as ferramentas de edição modernas? Ou talvez criar um formulário robusto para aplicar provas ou fazer pesquisas? Não se preocupe, o PRACTICE criou materiais para ajudar com isso.</p>
      </div>
      <div class="col-md-5">
        <p><img alt="image" class="img-fluid" src="/images/icons/undraw_content_team_3epn.svg"></p>
      </div>
    </div>
  </div>
</section>

<section class="fdb-block">
  {% assign resources = site.data.resources | where: "active", true %}
  {% for resource in resources %}
    <div class="container">
      <div class="row align-items-center pt-2">
        {% include resource-list.html %}
      </div>
    </div>
  {% endfor %}
</section>

