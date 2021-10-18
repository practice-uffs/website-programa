---
layout: hero
title: "Parcerias"
image:
    feature: banner-rotulo.png
permalink: /parcerias/
---

<section class="mb-5">
    <div class="">
        <div class="row align-items-center pt-2">
            <div class="col-9">
                <h1>{{ page.title }}</h1>
                <h2>Vamos colaborar em projetos maiores?</h2>
                <p class="lead">Estamos sempre em busca ou disponíveis para parcerias.</p>
            </div>
            <div class="col-3">
                <img src="/images/illustrations/undraw_collab.svg" title="Pessoa sentada colaborando com outra pessoa em cadeira de rodas." />
            </div>
        </div>
    </div>
</section>

<p>Projetos grandes geralmente precisam de muitas mentes para serem executados. Uma das missões do programa é fomentar esse diálogo e troca de ideias, visdando garantir que todas elas tenham uma chance. Desde que o programa foi fundado, fizemos parcerias com diversas entidades e setores da UFFS para trabalhar em projetos maiores e mais ambiciosos.</p>
<p>Veja a lista abaixo dos nossos parceiros.</p>

{% assign partnerships = site.data.partnerships | where: "type","partnerships" %}

<section class="text-gray-600 body-font py-5">
    <div class="flex flex-col">
        {% assign active_partnerships = partnerships | where: "active",true %}
        {% for partnership in active_partnerships %}
            {% include partnership-list.html %}
        {% endfor %}
    </div>
</section>
