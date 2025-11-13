---
layout: home
---

<div class="posts-list">
  {% for post in site.posts %}
    <article class="post-item">
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
      <a href="{{ post.url | relative_url }}">Read more</a>
    </article>
  {% endfor %}
</div>
