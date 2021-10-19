---
layout: hero
title: "Tecnologias"
image:
    feature: banner-rotulo.png
permalink: /tecnologias/
---

<section class="fdb-block">
    <div class="container">
        <div class="row align-items-center pt-2">
            <div class="col-12 col-md-8 col-lg-7">
                <h1>Tecnologias</h1>
                <h2>Nosso repertório de soluções</h2>
                <p class="lead">Trabalhamos continuamente para criar soluções tecnológicas para a comunidade acadêmica (e externa). Todas as soluções são de código aberto (open-source) e gratuitas.</p>
                <p class="text-sm text-gray-400">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                    Veja o código-fonte e documentação técnica das soluções em nosso <a href="https://github.com/practice-uffs" class="text-gray-400 underline">Github</a>.
                </p>
            </div>
            <div class="col-md-3 mt-6">
                <img src="/images/illustrations/undraw_Collaborators.svg" title="Ilustração de duas pessoas trabalhando juntas" />
            </div>
        </div>
    </div>
</section>

<section class="fdb-block">
    <div class="container text-justify">
        <p>O PRACTICE possui um conjunto de soluções tecnológicas prontas para uso, bem como várias em desenvolvimento (ou experimentação). Seguimos a ideia que software (e soluções tecnológicas) podem beneficiar a sociedade quando disponibilizadas de forma grauita e aberta.</p>
        
        <p>Prezamos pela transferência tecnológica daquilo que criamos, visando legitimamente colocar as pessoas no centro do processo. Nossas soluções visam sua utilização naquilo que as pessoas já possuem (como smartphones), de forma rápida e intuitiva. É a solução quem serve o usuário, não o contrário.</p>

        <div class="text-md text-gray-400 grid grid-cols-4 gap-1 py-4">
            <div class="col-span-3">Os softwares e soluções tecnológicas desenvolvidas no contexto do programa foram financiados com bolsas custeadas por verba Pública. Nosso entendimento sobre isso é que essas soluções precisam ser abertas, gratuitas e disponíveis para toda a comunidade.</div>
            <div>
                <svg xmlns="http://www.w3.org/2000/svg" class="w-20 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
                </svg>
            </div>            
        </div>

        <p>Seguimos o modelo <a href="https://pt.wikipedia.org/wiki/C%C3%B3digo_aberto" target="_blank">open-source</a> de desenvolvimento. Isso significa que todos nossos códigos-fonte (o que compõe os softwares) são aberto, acessíveis e modificáveis por qualquer pessoa. As ferramentas e tecnologias que utilizamos também são open-source. Tudo que criamos pode ser adaptado para diferentes contextos ou necessidades, sem autorização ou aquisição.</p>
        
        <p class="font-medium mt-5">Nossas soluções</p>

        <p>Conheça na lista abaixo nossas soluções e os projetos tecnológicos que estamos trabalhando.</p>

        <section class="text-gray-600 body-font overflow-hidden">
            {% for technology in site.data.technologies %}
                {% include technology-list.html %}
            {% endfor %}
        </section>
    </div>
</section>