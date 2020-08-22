---
layout: servicos
title: "Portfólio"
image:
  feature: banner-rotulo.png
permalink: /portfolio
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

{% assign portfolios = site.data.portfolio %}

<section>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-12 text-left">
        <h3>Portfólios do programa de Inovação PRACTICE</h3>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">
          {% assign active_portfolios = portfolios | where: "active",true %}
          {% for post in active_portfolios %}
            <hr />
            {% include post-partnerships.html %}
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</section>