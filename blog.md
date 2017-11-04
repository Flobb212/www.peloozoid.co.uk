---
layout: default
---

Click a post title to view in in full!


<html>
  {% for post in site.posts %}
    <article>
      <h1>
        <a href="{{post.url}}"> {{post.title}} </a> + - +
        <time date="{{post.date}}">{{post.date | date: '%d %B, %Y'}}</time>
      </h1>      
      {{post.excerpt}}
      <a href="{{ post.url }}">Read more</a>
    </article>
  {% endfor %}
</html>
