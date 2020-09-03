---
layout: hero
permalink: /
title: "Inicial"
image:
  feature: banner-rotulo.png
---

<section class="fdb-block" data-block-type="features" data-id="3" >
  <div class="container">
      <div class="row text-center justify-content-center mt-5">
          <div class="col-12 col-sm-4 col-xl-3 m-md-auto">
              <img alt="image" class="fdb-icon pb-4" width="60"
                  src="https://cdn.jsdelivr.net/gh/froala/design-blocks@master/dist/imgs//icons/map-pin.svg">
              <h3><strong>Consulta</strong></h3>
              <p>Qualidade das águas subterrâneas, superficiais e de abastecimento do Estado do Rio Grande do Sul.</p>
          </div>
          <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
              <img alt="image" class="fdb-icon pb-4" width="60"
                  src="https://cdn.jsdelivr.net/gh/froala/design-blocks@master/dist/imgs//icons/layers.svg">
              <h3><strong>Dados confiáveis</strong></h3>
              <p>Consulte os dados de qualidade do corpo d'água publicados em diversos trabalhos científicos.</p>
          </div>
          <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
              <img alt="image" class="fdb-icon pb-4" width="60"
                  src="https://cdn.jsdelivr.net/gh/froala/design-blocks@master/dist/imgs//icons/cloud.svg">
              <h3><strong>Monitoramento</strong></h3>
              <p>Compare o valor que consta na legislação e medições de qualidade de água observadas por pesquisadores.</p>
          </div>
      </div>
  </div>
</section>
<section class="fdb-block" data-block-type="contents" data-id="4" >
  <div class="container">
      <div class="row">
          <div class="col text-left">
              <h2>O que é esse serviço?</h2>
              <p>A <a href="https://www.uffs.edu.br">Universidade Federal da Fronteira Sul - UFFS</a>, através de seu corpo docente e de estudantes pesquisadores dos cursos de Engenharia Ambiental e Sanitária e Ciência da Computação, criou esse serviço online gratuíto para divulgação dos dados de qualidade das águas subterrâneas, superficiais e de abastecimento do Estado do Rio Grande do Sul.</p>
              <p>Esse serviço permite que qualquer entidade, seja cidadão ou órgão público, consulte os dados de qualidade do corpo d'água de seu interesse, publicados em diversos trabalhos científicos. Além disso, também é possível verificaros parâmetros de qualidade do corpo d'água que constam na legislação federal e estadual. Assim, todos podem comparar o valor que consta na legislação e o valor que têm sido observado por pesquisadores da área.</p>
          </div>
      </div>
  </div>
</section>
<section class="fdb-block">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-10 col-sm-6 col-md-5 col-lg-4 m-auto pb-5 pb-md-0">
        <img alt="image" class="img-fluid rounded-0" src="https://cdn.jsdelivr.net/gh/froala/design-blocks@master/dist/imgs/draws/iphone-hand.svg">
      </div>
      <div class="col-12 ml-md-auto col-md-7 col-lg-6 pb-5 pb-md-0">
        <h2>Aplicativo móvel</h2>
        <p class="lead">Confira a qualidade das águas onde você estiver utilizando seu smartphone.</p>
        <p>Todas as informações contidas nessa página estão disponíveis para consulta através do nosso aplicativo Qualidade das Águas. Além de pesquisar pelo nome, você também pode utilizar a sua localização para obter informações sobre a qualidade da água deste local.</p>
        <p class="mt-4">
          <a class="btn btn-primary" href="#"><i class="fab fa-google-play"></i> Google Play</a>
        </p>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="card breath-top">
    <div class="card-header">
      <h3>Destaques</h3>
    </div>
    <div class="card-body">
      <div class="row justify-content-center">
        <div class="col-12">
          <div class="tiles">
            {% assign highlighted-posts = site.categories.noticias | where: "highlight","true" | sort:"highlight_order" %}
            {% for post in highlighted-posts limit: 4 %}
              {% include post-grid.html %}
            {% endfor %}
          </div><!-- /.tiles -->
        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="card breath-top">
    <div class="card-header">
      <h3>Últimas notícias</h3>
    </div>
    <div class="card-body">
      <div class="row">
        <div class="col-12 text-left">
          {% for post in site.categories.noticias %}
            {% if post.highlight == false %}
              {% include post-grid-mini.html %}
            {% endif %}
          {% endfor %}
        </div>
      </div>
      <div class="row">
        <div class="col-12 text-right">
          <a href="/noticias">Ver mais notícias</a>
        </div>
      </div>
    </div>
  </div>
</section>
