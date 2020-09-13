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
              <img alt="image" class="fdb-icon pb-4" width="65"
                  src="/images/icons/brain.png">
              <h3><strong>Tecnologia</strong></h3>
              <p>Buscamos criar soluções tecnológicas para aprimorar o ambiente acadêmico de ensino e aprendizagem.</p>
          </div>
          <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
              <img alt="image" class="fdb-icon pb-4" width="60"
                  src="/images/icons/group.png">
              <h3><strong>Comunidade</strong></h3>
              <p>Não estamos sós, focamos na habilidade pedagógica e tecnológica tanto de servidores quanto estudantes.</p>
          </div>
          <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
              <img alt="image" class="fdb-icon pb-4" width="68"
                  src="/images/icons/fist.png">
              <h3><strong>Independência</strong></h3>
              <p>Nossa missão é empoderar tecnologicamente pessoas para que a tecnologia seja ajuda, não barreira.</p>
          </div>
      </div>
  </div>
</section>
<section class="fdb-block" data-block-type="contents" data-id="4" >
  <div class="container">
      <div class="row">
          <div class="col text-left">
              <h2>O que é o PRACTICE?</h2>
              <p>O Programa de Ampliação e Consolidação de Tecnologias e Inovação no Contexto Educacional (PRACTICE) objetiva estruturar ambientes e capacitar agentes educacionais para a produção e mediação de conteúdos por meio de tecnologias. Visamos contribuir para a promoção da inovação no processo de ensino-aprendizagem da UFFS, seja em componentes curriculares e extracurriculares, projetos ou iniciativas.</p>
              <h3>O que fazemos?</h3>
              <p>Capacitação didática de docentes para a oferta de aulas via telepresença, de maneira síncrona e assíncrona, bem como o fomento para o desenvolvimento de tecnologias inovadoras próprias da UFFS voltadas à interação, criação, curadoria e distribuição de conteúdos de acesso público.</p>
              <p>Também trabalhamos pelos estudantes para que tenham voz de sugestão de adequação de programas de Assistência Estudantil para oportunizar a participação de todos, sem prejuízo, nas atividades de envolvam tecnologia.</p>
              <h3>Como fazemos e trabalhamos?</h3>
              <p>Trabalhamos pela estruturação de ambientes que possibilitem a gravação, transmissão, edição e produção de conteúdos educacionais nas mais variadas plataformas de distribuição de conteúdo. Nossas soluções incluem, por exemplo, adaptação de algumas salas de aulas atuais da UFFS para o oferecimento de aula em tempo real por telepresença.</p>
              <p>Todo nosso trabalho é feito de forma pública e transparente através do <a href="https://github.com/practice-uffs" target="_blank">Github</a>. Nossas soluções tecnológicas são open-souce, livres para todos usarem. Nossos materiais são gratuítos e reutilizáveis ou adaptáveis. Acreditamos que a inovação aberta, com ciência e tecnologia a favor da comunidade, fará a diferença no avanço da educação.</p>
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
        <p class="lead">Todas nossas soluções são acessíveis através de nosso aplicativo para smartphones.</p>
        <p>Queremos que a tecnologia chegue até servidores e estudantes de forma fácil, sem complicações. Queremos ferramentas na palma da mão de cada um dos membros de nossa comunidade acadêmica. Trabalhamos para que nossos avanços estejam disponíveis, em primeira mão, em seu celular, para um uso fácil e imediato.</p>
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
            {% assign highlighted-posts = site.categories.noticias | where: "highlight","true" %}
            {% for post in highlighted-posts limit: 4 %}
              {% include post-news.html %}
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
