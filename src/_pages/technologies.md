---
layout: hero
title: "Tecnologias"
image:
  feature: banner-rotulo.png
permalink: /tecnologias/
---

<section class="fdb-block">
  <div class="container">
    <h2 class="pb-5">Tecnologias</h2>
    {% assign active_tools = site.data.technologies %}
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

