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
        <p class="lead">Precisa realizar uma videoconferência e não sabe qual a melhor forma de fazer? Precisa fazer um vídeo, animação ou imagem e tem dificuldade em lidar com as ferramentas de edição modernas? Ou talvez criar um formulário robusto para aplicar provas ou fazer pesquisas? <b>Não se preocupe</b>, o PRACTICE elaborou vários recursos incríveis para facilitar sua vida e melhorar a sua curva de aprendizado!</p>
      </div>
      <div class="col-md-5">
        <p><img alt="image" class="img-fluid" src="/images/montanhas_practice.png"></p>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="col-md-12">
      {% assign resources = site.data.resources | where: "active", true %}
      {% for resource in resources %}
        {% include resource-list.html %}
      {% endfor %}
    </div>
  </div>
</section>