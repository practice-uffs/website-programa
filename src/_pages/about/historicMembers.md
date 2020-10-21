---
layout: hero
title: "Histórico de Membros"
image:
  feature: banner-rotulo.png
permalink: /equipe/historico/
---

<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center pt-2">
      <div class="col-12 col-md-8 col-lg-7">
        <h2>Histórico de Membros</h2>
        <p class="lead">Aqui você encontra todas as pessoas que fizeram ou fazem parte dessa equipe maravilhosa. Todos que já contribuiram e podem contribuir muito com o PRACTICE.</p>
      </div>
      <div class="col-md-3 mt-6">
          <lottie-player alt="image" class="fdb-icon pb-4" src="https://assets3.lottiefiles.com/packages/lf20_P9ArQ8.json"  background="transparent"  speed="1"  style="width: 400px; height: 400px;" loop autoplay></lottie-player>
      </div>
    </div>
  </div>
</section>

<table class="table table-striped">
  <thead>
    <tr>
      <th scope="col">Nome</th>
      <th scope="col">Vínculo</th>
      <th scope="col">Equipe</th>
      <th scope="col">Tempo de atuação</th>
    </tr>
  </thead>
  <tbody>
    {% assign people = site.data.people | sort:"name" %}
    {% for person in people %}
      <tr>
        <td scope="row">{{ person.name }}</td>
        <td>{{ person.bond }}</td>
        <td>{{ person.position }}</td>
        <td>{{ person.actingTime }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>