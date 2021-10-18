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
        <h1>Equipe</h1>
        <h2>Quem são as pessoas</h2>
        <p class="lead">O PRACTICE conta com um grupo de estudantes e servidores multidisciplinar e multicampi para realizar diversos tipos de atividades.</p>
        <p class="text-sm text-gray-400">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            Conheça o <a href="/equipe/historico/" class="text-gray-400 underline">histórico de integrantes</a> do programa.
        </p>
      </div>
      <div class="col-md-3 mt-6">
          <img src="/images/illustrations/undraw_collaborators.svg" title="Ilustração de duas pessoas trabalhando juntas" />
      </div>
    </div>
  </div>
</section>

<section class="fdb-block">
  <div class="container">
    <section class="pt-1">
      <h2 class="pb-3">Coordenação</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign active = site.data.people | where:"position","coor-geral" %}
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
        {% assign active = site.data.people | where:"position","con-conteudo" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Transmissões ao vivo</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","con-midia-live" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Áudio, vídeo e animações</h3>
      <div class="card-group">
        {% assign active = site.data.people | where:"position","con-midia-AVA" %}
        {% assign people = active | where:"person","true" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Desenvolvimento de software</h2>
      <hr class="pb-4">
      <div class="card-group space-y-2">
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
      <h2 class="pb-3">Auxílio Gerencial</h2>
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