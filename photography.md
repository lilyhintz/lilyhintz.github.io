---
layout: default
title: Photography
permalink: /photography/
---

<section class="gallery-page">

  <h1 class="gallery-title">
    PHOTOGRAPHY
  </h1>

  <div class="gallery-grid">

    {% assign photo_posts = site.posts | where: "category", "photography" %}

    {% for post in photo_posts %}

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