---
layout: servicos
title: "Portfólio"
image:
  feature: banner-rotulo.png
permalink: /portfolio/
---

<section class="fdb-block">
    <div class="container">
      <h1 class="text-center"><b>{{ page.title }}</b></h1>
      <div class="row align-items-center pt-0">
        <div class="col-8 col-md-6 m-auto m-md-0 ml-md-auto pt-3">
          <img style="width: 480px; height: 280px; border-radius: 5px;" class="card-img-top" src="/images/illustrations/undraw_Portfolio_update_re_jqnp.png">
        </div>
        <div class="col-12 col-md-4 col-lg-6 pt-4">
          <p class="lead text-justify">O PRACTICE conta com um amplo portfólio de atividades realizadas, dentre elas se destacam as transmissões ao vivo auxiliadas e os diversos vídeos editados. A equipe do programa trabalha com comprometimento e seriedade, visando garantir o nível de excelência exigido. Alguns dos materiais produzidos podem ser visualizados abaixo:</p>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row align-items-center pt-2">
        <div class="col-12 col-md-5 col-lg-6">
          <h2 class="text" style="color: #00384d;">Transmissões ao vivo</h2>
          <p class="lead text-justify">O PRACTICE oferece auxílio na produção e realização de eventos, com organização e transmissão online. Nossa equipe utiliza 
          tecnologias como o OBS Studio, que permite a execução de transmissões ao vivo com alta qualidade e confiabilidade. Utilizamos também o Cisco Webex, oferecido pela universidade para melhor qualidade de vídeo e áudio dos ministrantes.</p>
        </div>
        <div class="col-8 col-md-5 m-auto m-md-5 ml-md-auto pt-2">
          <img style="width: 480px; height: 250px; border-radius: 5px;" class="card-img-top" src="/images/portfolio/4_3.jpg">
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row align-items-center pt-2">
        <div class="col-8 col-md-6 m-auto m-md-0 ml-md-auto pt-5">
          <a href="https://youtu.be/zLT9UG_GSZI" target="_blank"> 
            <img style="width: 480px; height: 250px; border-radius: 5px;" class="card-img-top" src="/images/portfolio/portfolio_overley.png">
            <p style="font-size: 15px;">Clique e assista a essa transmissão.</p>
          </a>
        </div>
        <div class="col-12 col-md-4 col-lg-6">
          <h2 class="text" style="color: #00384d;">Overlay de transmissões</h2>
          <p class="lead text-justify">O pratice conta também com materiais personalizados próprios, como o overlay de lives, que nada mais é do que a identidade visual de nossas transmissões. Tal identidade deixa os eventos auxiliados pelo programa ainda mais organizados, onde é possível visualizar o chat da transmissão em tempo real e as apresentações dos ministrantes de forma eficiente.</p>
        </div>
      </div>
    </div>
</section>

{% assign portfolios = site.data.lives %}

<section>
  <div class="card breath-top">
    <div class="card-header">
      <h3>Algumas das transmissões realizadas recentemente:</h3>
    </div>
    <div class="card-body">
      <div class="row">
        <div class="col-12 text-left">
          {% assign active_portfolios = portfolios | where: "portfolio","true" %}
          {% for flyer in active_portfolios reversed %}
            {% include portfolio-list.html %}
          {% endfor %}
        </div>
      </div>
      <div class="row">
        <div class="col-12 text-right">
          <a href="/portfolio/lives/">Ver todas as transmissões</a>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="fdb-block">
    <div class="container">
      <div class="row align-items-center pt-5">
        <div class="col-12 col-md-5 col-lg-6">
          <h2 class="text" style="color: #00384d;">Gravações em estúdio (temporariamente suspenso devido ao NSO dos campi)</h2>
          <p class="lead text-justify">O PRACTICE oferece também os serviços de produção e edição de vídeos. Nossa equipe está preparada para transformar uma proposta de vídeo em realidade, como vídeos de divulgação e até aulas. Os vídeos produzidos pelo programa são acessíveis e podem contar com todos mecanismos necessários para que todos os públicos possam assisti-los.</p>
        </div>
        <div class="col-8 col-md-5 m-auto m-md-5 ml-md-auto pt-5">
          <a href="https://youtu.be/0optATn6jW8" target="_blank">
            <img style="width: 480px; height: 250px; border-radius: 5px;" class="card-img-top" src="/images/portfolio/K1g4Nn.gif">
            <p style="font-size: 15px;">Clique e acesse ao vídeo.</p>
          </a>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row align-items-center pt-2">
        <div class="col-8 col-md-6 m-auto m-md-0 ml-md-auto pt-5">
          <a href="https://fb.watch/7qtgl3bcTv/" target="_blank"> 
            <img style="width: 480px; height: 250px; border-radius: 5px;" class="card-img-top" src="/images/portfolio/colação_de_grau.png">
            <p style="font-size: 15px;">Clique e assista a essa transmissão.</p>
          </a>
        </div>
        <div class="col-12 col-md-4 col-lg-6">
          <h2 class="text" style="color: #00384d;">Colação de Grau Remota</h2>
          <p class="lead text-justify">O PRACTICE atuou no apoio técnico e produção de um dos eventos mais esperados por quem ingressa na graduação - a colação de grau! No contexto pandêmico, onde se fez (e ainda faz) necessário o distânciamento social, um evento como esse precisa ser reinvetado e adaptado, e o PRACTICE está à diposição para colaborar nesse novo cenário.</p>
        </div>
      </div>
    </div>
</section>

<section class="fdb-block pt-5">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-10 col-lg-6">
        <p><img style="border-radius: 5px;" alt="image" class="img-fluid" src="/images/portfolio/4_2.jpg"></p>
      </div>
      <div class="col-10 col-lg-6">
        <p><img style="border-radius: 5px;" alt="image" class="img-fluid" src="/images/portfolio/IMG_4127.JPG"></p>
      </div>
    </div>
  </div>
</section>