---
layout: hero
title: "Notícias"
date: 2014-05-30T11:39:03-04:00
tags: []
image:
  feature: banner-rotulo.png
---
<article>
  <div class="page-title">
    <h1>Notícias</h1>
    <hr />
  </div>
  <div class="tiles">
    {% for post in site.categories.noticias %}
      {% include post-news.html %}
    {% endfor %}
  </div>
</article>