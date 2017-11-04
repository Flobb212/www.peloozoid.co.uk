---
layout: default
---

<html>
  {% for post in site.posts %}
    <article class="blogPosts">
      <h1>
        <a href="{{post.url}}"> {{post.title}} </a>
        <time date="{{post.date}}">{{post.date | date: '%d %B, %Y'}}</time>
      </h1>      
      {{post.excerpt}}
      <a href="{{ post.url }}">Read more</a>
    </article>
  {% endfor %}
</html>
