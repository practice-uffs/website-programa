---
layout: hero
title: "Ferramentas"
image:
  feature: banner-rotulo.png
permalink: /ferramentas/
---


<section class="fdb-block">
  <div class="container">
    <h2 class="pb-5">Ferramentas</h2>
    {% assign active_tools = site.data.tools %}
    <ul id="profileTabs" class="nav nav-tabs justify-content-center nav-justified">
        {% for tool in active_tools %}
          {% include tool-list.html %}
        {% endfor %}
    </ul>
    <div class="tab-content pt-3">
        {% for tool in active_tools %}
          {% include tool.html %}
        {% endfor %}
    </div>
  </div>
</section>

