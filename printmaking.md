---
layout: default
title: Printmaking
permalink: /printmaking/
---

<section class="gallery-page">

  <h1 class="gallery-title">
    PRINTMAKING
  </h1>

  <div class="gallery-grid">

    {% assign print_posts = site.posts | where: "category", "printmaking" %}

    {% for post in print_posts %}

      <a class="gallery-card" href="{{ post.url }}">

        <img
          src="{{ post.hero_image }}"
          alt="{{ post.title }}"
        >

        <div class="gallery-card-meta">
          {{ post.date | date: "%Y" }}
        </div>

        <h2>
          {{ post.title | upcase }}
        </h2>

      </a>

    {% endfor %}

  </div>

</section>