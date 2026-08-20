---
layout: default
title: Meu Blog
---

# Meu Blog

Bem-vinda ao meu espaço de artigos sobre tecnologia, dados e programação.

## Artigos

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: "%d/%m/%Y" }}

{{ post.excerpt | strip_html | truncatewords: 35 }}

[Leia a matéria →]({{ post.url | relative_url }})

---
{% endfor %}
