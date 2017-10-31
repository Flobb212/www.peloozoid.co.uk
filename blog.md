---
layout: default
---

<html>
  {% for post in site.posts %}
    <article>
      <h1>
        <a href="{{post.url}}">
          {{post.title}}
        </a>
      </h1>
      <time datetime="{{post.Date}}">{{post.Date}}</time>
      {{post.content}}
    </article>
  {% endfor %}
</html>
