---
layout: servicos
title: "Parcerias"
image:
  feature: banner-rotulo.png
permalink: /parcerias
---

<div class="container">
    <div class="row align-items-center pt-2">
        <div class="col-md-7">
            <h2>Parcerias</h2>
        </div>
    </div>
</div>


{% assign projects = site.data.projects | where: "type","project-extension" %}

<section>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-12 text-left">
        <h3>Projetos em andamento</h3>
        <hr />
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">
          {% assign active_projects = projects | where: "active",true | sort:"date_start" | reverse %}
          {% for post in active_projects %}
            {% include post-grid-mini.html %}
          {% endfor %}
        </div><!-- /.tiles -->
      </div>
    </div>
  </div>
</section>

{% assign inactive_projects = projects | where: "active",false %}

<section>
  <div class="container breath-top">
    <div class="row justify-content-center">
      <div class="col-12 text-left">
        <h3>Projetos finalizados</h3>
        <hr />
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12">
        <div class="tiles">
          {% assign inactive_projects = projects | where: "active",false | sort:"date_end" | reverse %}
          {% for post in inactive_projects %}
            {% include post-grid-mini.html %}
          {% endfor %}
        </div><!-- /.tiles -->
      </div>
    </div>
  </div>
</section>