---
layout: default
title: Poetry
permalink: /poetry/
---

<section class="archive-page">

  <h1 class="archive-title">
    POETRY
  </h1>

  <div class="archive-list">

    {% assign poetry_posts = site.posts | where: "category", "poetry" %}

    {% for post in poetry_posts %}

      <a class="archive-item" href="{{ post.url }}">

        <div class="archive-item-title">
          {{ post.title | upcase }}
        </div>

        <div class="archive-item-meta">
          {{ post.journal }} / {{ post.date | date: "%B %-d, %Y" }}
        </div>

      </a>

    {% endfor %}

  </div>

</section>