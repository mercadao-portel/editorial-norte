---
layout: default
title: Editorial Norte
---

<div class="container">

# Editorial Norte
Bem-vindo ao nosso portal de notícias!

Aqui você encontra nossas matérias publicadas diariamente.  

## Últimas Matérias

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>:
      <a href="{{ post.url }}">{{ post.title }}</a>
      {% if post.excerpt %}
        <p>{{ post.excerpt }}</p>
      {% endif %}
      {% if post.image %}
        <img src="{{ post.image }}" alt="{{ post.title }}" class="post-image"/>
      {% endif %}
    </li>
  {% endfor %}
</ul>

</div>
