---
layout: hero
permalink: /
title: "Inicial"
excerpt: 'Conheça o PRACTICE, um programa de ensino, pesquisa, extensão e inovação da Universidade Federal da Fronteira Sul (UFFS), composto por bolsistas e professores que atuam com o objetivo de empoderar tecnologicamente a comunidade acadêmica.'
image:
    feature: banner-rotulo.png
---

<section class="fdb-block">
    <div class="container">
        <div class="row text-center justify-content-center mt-5">
            <div class="col-12 col-sm-4 col-xl-3 m-md-auto">
                <img src="/images/illustrations/undraw_visionary_technology.svg" class="h-36 mx-auto mb-8" title="Ilustração de uma pessoa frente a um smartphone com tecnologia visionária"/>
                <p class="font-light text-2xl">Tecnologia</p>
                <p class="text-sm">Buscamos criar soluções tecnológicas para aprimorar o ambiente acadêmico de ensino e aprendizagem.</p>
            </div>
            <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
                <img src="/images/illustrations/undraw_the_world_is_mine.svg" class="h-40 mx-auto mb-4 " title="Ilustração de uma pessoa carregando o planeta terra"/>
                <p class="font-light text-2xl">Comunidade</p>
                <p class="text-sm">Não estamos sós, focamos na habilidade pedagógica e tecnológica tanto de servidores quanto estudantes.</p>
            </div>
            <div class="col-12 col-sm-4 col-xl-3 m-auto pt-4 pt-sm-0">
                <img src="/images/illustrations/undraw_powerful.svg" class="w-42 mx-auto mb-6" title="Ilustração de uma pessoa carregando o planeta terra"/>
                <p class="font-light text-2xl">Independência</p>
                <p class="text-sm">Nossa missão é empoderar tecnologicamente pessoas para que a tecnologia seja ajuda, não barreira.</p>
            </div>
        </div>
    </div>
</section>

<section class="text-gray-600 body-font">
    <div class="container mx-auto flex px-5 py-5 md:flex-row flex-col items-center">
        <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 mb-10 md:mb-0">
            <lottie-player src="https://assets6.lottiefiles.com/packages/lf20_yoatyllj.json" background="transparent" speed="1"  style="width: 100%; height: auto;" loop autoplay></lottie-player>
        </div>
        <div class="lg:flex-grow md:w-1/2 lg:pl-24 md:pl-16 flex flex-col md:items-start md:text-left items-center ">
            <p class="font-extralight text-3xl">O que é?</p>
            <p class="mb-8 leading-relaxed text-gray-600">
                O PRACTICE é um programa de ensino, pesquisa, extensão e inovação da <a href="https://www.uffs.edu.br">Universidade Federal da Fronteira Sul (UFFS)</a>. Ele é composto por bolsistas e professores que atuam com o objetivo de empoderar tecnologicamente a comunidade acadêmica.
            </p>
            <p class="text-sm text-gray-400">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
                <a href="/equipe" class="text-gray-400 no-underline">Conheça a equipe</a>.
            </p>
        </div>
    </div>
</section>

<section class="text-gray-600 body-font">
    <div class="container mx-auto flex px-5 py-5 md:flex-row flex-col items-center">
        <div class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center">
            <p class="font-extralight text-3xl">Qual o objetivo?</p>
            <p class="mb-8 leading-relaxed  text-gray-600">
                O programa visa estruturar ambientes, capacitar agentes educacionais, produzir e mediar a produção de conteúdos educacionais. A filosofia é promover e democratizar tecnologia e inovação, do cotidiano até o processo de aprendizagem, de estudantes e servidores da UFFS.
            </p>
            <p class="text-sm text-gray-400">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
                Veja nossas <a href="/tecnologias" class="text-gray-400 no-underline">tecnologias e projetos</a>.
            </p>
        </div>
        <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
            <lottie-player src="https://assets1.lottiefiles.com/packages/lf20_2n1snrke.json"  background="transparent"  speed="1"  style="width: 90%; height: auto;"  loop autoplay></lottie-player>
        </div>
    </div>
</section>

<p>Como solicitar transmissões ao vivo:</p>
<img src="/images/fluxodelive.png" alt="Como solicitar transmissões ao vivo">

<h2 class="mt-10">Destaques</h2>
<hr />

<section class="text-gray-600 body-font overflow-hidden">
    <div class="py-8 mx-auto">
        <div class="flex flex-wrap -m-12">
            {% assign highlighted-posts = site.categories.noticias | where: "highlight","true" %}
            {% for post in highlighted-posts limit: 2 %}
            {% include post-news.html %}
            {% endfor %}
        </div>
    </div>
</section>

<h3 class="mt-24">Últimas notícias</h3>
<hr />

<section class="text-gray-600 body-font">
    <div class="py-2 mx-auto">
        <div class="flex flex-wrap -m-4">
            {% for post in site.categories.noticias %}
            {% if post.highlight == false %}
            {% include post-grid-mini.html %}
            {% endif %}
            {% endfor %}
        </div>
        <a href="/noticias" class="mt-4">Ver mais notícias</a>
    </div>
</section>