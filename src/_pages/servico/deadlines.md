---
layout: servicos
title: "Prazos de solicitação"
image:
    feature: banner-rotulo.png
permalink: /servico/prazos-de-solicitacao/
---

<section class="fdb-block">
    <div class="container">
        <div class="row align-items-center pt-2">
            <div class="col-12 col-md-9">
                <h1>Prazo de solicitação</h1>
                <h2>Conheça nosso tempo médio de trabalho</h2>
                <p class="lead">Qualquer um dos nossos serviços exige um solicitação com antecedência mínima, que depende de cada serviço.</p>
            </div>
            <div class="col-md-3 mt-6">
                <img src="/images/illustrations/undraw_schedule.svg" title="Ilustração de uma mulher em frente a um quadro" />
            </div>
        </div>
    </div>
</section>

<p>A partir do momento em que recebemos o pedido do solicitante, temos um prazo para fazer a análise do pedido. Durante esse período, verificaremos se a solicitação possui todas as informações e arquivos necessários para a realização do pedido. Isso está de acordo com o padrão estabelecido (que você pode conferir nas páginas de serviço do nosso site) e para as demais necessidades que abrangem o início do atendimento.</p>

<p>Além disso, caso o pedido não esteja completo e bem explicado, ele será retornado ao solicitante com solicitação das informações que precisam ser preenchidas. Pode-se, ainda, ser feito o agendamento de uma reunião para o esclarecimento do que foi solicitado, para que o seu pedido possa entrar na fila de atendimento.</p>

<p>Ao iniciar o atendimento teremos um prazo para produzir e entregar seu produto. Lembre-se que várias pessoas irão solicitar os serviços além de você. Pedir com antecedência garantirá que você receba seu produto no momento em que você deseja.</p>

<p>Em caso de eventuais adversidades (fora de nosso controle), os prazos de solicitação e produção podem ser prolongados. Similarmente, se tudo acontecer conforme o previsto, seu produto pode ficar pronto antes do prazo esperado.</p>

<p>Confira os prazos para cada um de nossos serviços na tabela abaixo.</p>

<table class="table table-striped">
    <thead>
        <tr>
            <th scope="col">PRODUTOS</th>
            <th scope="col">ID </th>
            <th scope="col">Níveis de complexidade para produtos </th>
            <th scope="col">Prazos de avaliação do pedido</th>
            <th scope="col">Prazos de produção com todos os materiais já enviados </th>
        </tr>
    </thead>
    <tbody>
        {% assign products = site.data.aplicationDeadlines %}
        {% for product in products %}
        <tr>
            <td scope="row">{{ product.product }}</td>
            <td>{{ product.id }}</td>
            <td>{{ product.description }}</td>
            <td>{{ product.evaluation_deadline }}</td>
            <td>{{ product.production_deadline }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>