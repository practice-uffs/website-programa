---
layout: servicos
title: "Portfólio"
image:
  feature: banner-rotulo.png
permalink: /portfolio/
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-12 col-md-8 col-lg-7">
        <h2>{{ page.title }}</h2>
        <p class="lead">Conheça os produtos e serviços que foram criados ou executados com o auxílio do programa.</p>
      </div>
      <div class="col-8 col-md-4 m-auto m-md-0 ml-md-auto pt-5">
        <p><img alt="image" class="img-fluid" src="/images/illustrations/undraw_Portfolio_update_re_jqnp.svg"></p>
      </div>
    </div>
  </div>
</section>

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-12">
        <h2>Eventos virtuais</h2>
      </div>
    </div>
    <div class="row align-items-center">
      <div class="col-10 col-lg-6">
        <p>O programa já auxiliou na execução de diversos eventos virtuais, como lives de capacitação de setores da universidade e semanas acadêmicas. Nossa equipe utiliza as melhores tecnologias e recursos para enriquecer as transmissões.</p>
      </div>
      <div class="col-10 col-lg-6">
        <p><img style="border-radius: 5px;" alt="image" class="img-fluid" src="/images/portfolio/4_3.jpg"></p>
      </div>
    </div>
  </div>
</section>

{% assign portfolios = site.data.portfolios %}

<section>
  <div class="container pb-5">
    <div class="row justify-content-center">
      <div class="col-12 text-left">
        <h3>Algumas das transmissões realizadas recentemente:</h3>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">
          {% assign active_portfolios = portfolios | where: "active",true | sort:"portfolio" %}
          {% for portfolio in active_portfolios reversed %}
            {% include portfolio-list.html %}
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</section>

<section class="fdb-block pt-5">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-12">
        <h2>Gravações em estúdio e vídeos</h2>
      </div>
    </div>
    <div class="row align-items-center">
      <div class="col-10 col-lg-6">
        <p><img style="border-radius: 5px;" alt="image" class="img-fluid" src="/images/portfolio/VID_20200903_095150497_013.jpg"></p>
      </div>
      <div class="col-10 col-lg-6">
        <p><img style="border-radius: 5px;" alt="image" class="img-fluid" src="/images/portfolio/IMG_4127.JPG"></p>
      </div>
    </div>
  </div>
</section>