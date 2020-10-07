---
layout: hero
title: "Equipe"
image:
  feature: banner-rotulo.png
permalink: /equipe/
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-12 col-md-8 col-lg-7">
        <h2>Equipe</h2>
        <p class="lead">O PRACTICE conta com uma equipe de estudantes e servidores que se dedicam de forma organizada e eficiente para realizar diversos tipos de atividades. <a href="/equipe/historic/">Histórico de membros PRACTICE.</a></p>
      </div>
      <div class="col-md-3 mt-6">
          <lottie-player alt="image" class="fdb-icon pb-4" src="https://assets10.lottiefiles.com/packages/lf20_CbwvP6/data.json"  background="transparent"  speed="1"  style="width: 400px; height: 400px;" loop autoplay></lottie-player>
      </div>
    </div>
  </div>
</section>



<section class="fdb-block">
  <div class="container">
    <section class="pt-1">
      <h2 class="pb-3">Coordenação</h2>
      <hr class="pb-4">
      <h3>Coordenação Geral</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","coor-geral" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Coordenação Técnica-pedagógica</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","coor-tec" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Produção de conteúdo</h2>
      <hr class="pb-4">
      <h3>Texto e imagem</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","con-material" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Imagem, vídeo e som</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","con-midia" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Desenvolvimento de software</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign active = site.data.people | where:"position","dev" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Design Gráfico</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign active = site.data.people | where:"position","con-design" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Auxílio organizacional</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign active = site.data.people | where:"position","ger-aux" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
  </div>
</section>