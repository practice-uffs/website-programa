---
layout: hero
title: "Parcerias"
image:
  feature: banner-rotulo.png
permalink: /parcerias
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-12 col-md-8 col-lg-7">
        <h2>Parcerias</h2>
        <p class="lead">Página destinada a parceiros do Programa de Inovação PRACTICE.</p>
      </div>
      <div class="col-8 col-md-4 m-auto m-md-0 ml-md-auto pt-5">
        <p><img alt="image" class="img-fluid" src="https://cdn.jsdelivr.net/gh/froala/design-blocks@2.0.1/dist/imgs//draws/git.svg"></p>
      </div>
    </div>
  </div>
</section>


{% assign partnerships = site.data.partnerships |  where: "type","partnerships" %}

<section>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-12 text-left">
        <h3>Parceiros do programa de Inovação PRACTICE</h3>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">
          {% assign active_partnerships = partnerships | where: "active",true | sort:"date_start" | reverse %}
          {% for post in active_partnerships %}
            <hr />
            {% include post-grid-mini.html %}
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</section>