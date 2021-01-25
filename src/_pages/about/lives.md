---
layout: servicos
title: "Transmissões ao vivo"
image:
  feature: banner-rotulo.png
permalink: /portfolio/lives/
---

<section class="fdb-block">
  <div class="container">
    <h1 class="text-center"><b>{{ page.title }}</b></h1>
    <div class="row align-items-center pt-0">
      <div class="col-8 col-md-6 m-auto m-md-0 ml-md-auto pt-3">
        <img style="width: 400px; height: 280px; border-radius: 5px;" class="card-img-top" src="/images/illustrations/undraw_online_media_62jb.png">
      </div>
      <div class="col-12 col-md-4 col-lg-6 pt-4">
        <p class="lead text-justify">O PRACTICE conta com um amplo portfólio de atividades realizadas, dentre elas se destacam as transmissões ao vivo auxiliadas e os diversos vídeos editados. A equipe do programa trabalha com comprometimento e seriedade, visando garantir o nível de excelência exigido. Alguns dos materiais produzidos podem ser visualizados abaixo:</p>
      </div>
    </div>
  </div>
</section>


{% assign lives = site.data.lives %}

<section>
  <div class="container pb-5">
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">

        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="card breath-top">
    <div class="card-header">
      <h3>Algumas das transmissões realizadas recentemente:</h3>
    </div>
    <div class="card-body">
      <div class="row">
        <div class="col-12 text-left">
          {% assign flyers = lives | sort: "flyer" %}
          {% for flyer in flyers reversed %}
            {% include portfolio-list.html %}
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</section>