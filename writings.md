---
layout: default
---
<h1>Latest Posts</h1>

<ul>
  {% assign total = 0 %}
  {% for post in site.posts %}
    {% assign total = total | plus: 1 %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
  (size: {{ total }})
</ul>