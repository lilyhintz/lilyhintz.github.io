---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

---
layout: home
title: Home
---

{% for post in site.posts %}
  <article class="home-post">
    <h2 class="home-post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p class="home-post-date">
      {{ post.date | date: "%Y" }}
    </p>
  </article>
{% endfor %}
