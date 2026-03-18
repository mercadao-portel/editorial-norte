
---
layout: default
title: Editorial Norte
---

# Editorial Norte

Bem-vindo ao nosso portal de notícias! Aqui você encontra nossas matérias publicadas diariamente.

## Últimas Matérias

{% for post in site.posts %}
- **{{ post.date | date: "%d/%m/%Y" }}:** [{{ post.title }}]({{ post.url }})
  {{ post.excerpt }}
{% endfor %}
