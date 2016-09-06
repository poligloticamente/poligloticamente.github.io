---
layout: page
title: Aprenda
permalink: /aprenda/
---

<div class="home">

  <h1 class="page-heading">Artigos sobre aprender a apreender</h1>

  <ul class="post-list">
    {% for post in site.categories.aprender %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
        {{ post.excerpt }}
      </li>
    {% endfor %}
</ul>
