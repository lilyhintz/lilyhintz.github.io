---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

---
layout: default
---

<h1 class="site-title">{{ site.title }}</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-list-date">
        {{ post.date | date: "%Y" }}
      </span>
    </li>
  {% endfor %}
</ul>
