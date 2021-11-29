---
layout: hero
title: "Portfólio"
image:
    feature: banner-rotulo.png
permalink: /portfolio/
---

<section>
    <div class="container">
        <div class="row align-items-center pt-2">
            <div class="col-12 col-md-8 col-lg-7">
                <h1>Portifólio</h1>
                <h2>Um pouco sobre nossos projetos realizados</h2>
                <p class="lead">Criamos e ajudados a executar muitos projetos, materiais e iniciativas. Conheça as principais delas.</p>
                <p class="text-sm text-gray-400">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                    Tudo que fazemos é gerenciado (e visível) publicamente em nosso <a href="https://github.com/practice-uffs" class="text-gray-400 underline">Github</a>.
                </p>
            </div>
            <div class="col-md-3 mt-6">
                <img src="/images/illustrations/undraw_creative_draft.svg" title="Ilustração de uma pessoa e um smartphone com aplicativos" />
            </div>
        </div>
    </div>
</section>

<section class="text-gray-600 body-font overflow-hidden mt-16">
    {% for portfolio in site.data.portfolio %}
        {% include portfolio-list.html %}
    {% endfor %}
</section>

{% assign portfolios = site.data.lives %}

<section class="mb-10">
    <div class="card breath-top">
        <div class="card-header">
            <h3>Algumas de nossas transmissões realizadas recentemente:</h3>
        </div>
        <div class="card-body">
            <div class="row">
                <div class="col-12 text-left">
                    {% assign active_portfolios = portfolios | where: "portfolio","true" %}
                    {% for flyer in active_portfolios reversed %}
                    {% include portfolio-list-live.html %}
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
