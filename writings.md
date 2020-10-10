---
layout: default
title: Blog
---
<ul>
  {% for post in site.posts %}
    <!-- <li> -->
    <date>{{post.date | date_to_string}}</date> <a href="{{ post.url }}">{{ post.title }}</a>  <br><br>
    <!-- </li> -->
  {% endfor %}
  <br>
  <br>
  <br>
  <br>
  <a style="font-style:italic;color:grey;" href="/feed.xml">
    <img alt="rss feed" width="12" height="12" srcset="/assets/images/rss.svg">
  </a>
</ul>

