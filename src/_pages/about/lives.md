---
layout: servicos
title: "Lives"
image:
  feature: banner-rotulo.png
permalink: /portfolio/lives/
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-12 col-md-8 col-lg-7">
        <h2>{{ page.title }}</h2>
        <p class="lead">Conheça todas as lives realizadas pelo PRACTICE.</p>
      </div>
      <div class="col-8 col-md-4 m-auto m-md-0 ml-md-auto pt-5">
        <p><img alt="image" class="img-fluid" src="/images/illustrations/undraw_Portfolio_update_re_jqnp.svg"></p>
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