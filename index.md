---
layout: default
title: Meu Blog
---

<section class="hero">

  <div class="hero-content">

    <div class="hero-label">
      BEM-VINDA AO MEU BLOG
    </div>

    <h1>
      Tecnologia que<br>
      gera impacto<span>.</span>
    </h1>

    <p class="hero-text">
      Aqui compartilho análises, estudos e aprendizados sobre
      tecnologia, dados e mercado de trabalho para transformar
      informação em conhecimento aplicado.
    </p>

    <a href="#artigos" class="hero-button">
      VER ARTIGOS →
    </a>

  </div>

  <div class="hero-image"></div>

</section>


<section class="articles-section" id="artigos">

  <div class="section-header">

    <div class="section-line"></div>

    <h2>ARTIGOS</h2>

    <p>
      Conteúdos sobre tecnologia, dados e mercado de trabalho.
    </p>

  </div>


  {% for post in site.posts %}

  <article class="post-card">

    <div class="post-image"></div>

    <div class="post-content">

      <div class="tags">

        <span class="tag">
          PESQUISA
        </span>

        <span class="tag">
          MERCADO DE TECNOLOGIA
        </span>

      </div>


      <h3>
        <a href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h3>


      <p class="post-description">

        Uma análise sobre linguagens de programação,
        adoção, crescimento, áreas de aplicação e
        perspectivas profissionais no mercado.

      </p>


      <div class="post-footer">

        <span class="post-date">
          {{ post.date | date: "%d %b %Y" | upcase }}
        </span>

        <a class="read-more"
           href="{{ post.url | relative_url }}">
          LER ARTIGO →
        </a>

      </div>

    </div>

  </article>

  {% endfor %}

</section>
