---
layout: default
---

<html>
  {% for post in site.posts %}
    <article class="blogPosts">
      <h1>
        <a href="{{post.url}}"> {{post.title}} </a> + - + {{post.date}}
      </h1>      
      {{post.excerpt}}
      <a href="{{ post.url }}">Read more</a>
    </article>
  {% endfor %}
</html>
