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
      <div class="col-12 col-md-8 col-lg-12">
        <h2>Prazo de solicitação de produtos</h2>
        <p class="lead">Para ter acesso a qualquer um dos serviços do PRACTICE é necessário realizar a solicitação com antecedência mínima (confira a tabela de prazos abaixo), a depender de cada serviço. A partir do momento em que recebemos o pedido do solicitante, temos um prazo para fazer a análise do pedido, no qual será verificado se a solicitação possui todas as informações e arquivos necessários para realizar o pedido, de acordo com o padrão estabelecido (que você pode conferir nas páginas de serviço do nosso site) e para as demais necessidades que abrangem o início do atendimento.
        Além disso, caso o pedido não esteja completo e bem explicado, será retornado ao solicitante com o pedido das informações que precisam ser preenchidas ou, ainda, pode ser feito o agendamento de uma reunião para o esclarecimento do que foi solicitado, para que o seu pedido possa entrar na fila de atendimento.
        Ao iniciar o atendimento teremos um prazo para produzir e entregar seu produto. Lembre-se que várias pessoas irão solicitar os serviços além de você, pedir com antecedência vai garantir que você receba seu produto no momento em que você deseja. 
        Devido à possíveis adversidades que possam ocorrer, os prazos de solicitação e produção podem ser prolongados, da mesma forma, se tudo acontecer conforme o previsto seu produto pode ficar pronto antes do prazo esperado.
        </p>
      </div>
    </div>
  </div>
</section>

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