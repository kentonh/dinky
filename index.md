---
layout: default
---

<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.date | date: "%B %-d, %Y" }}
      <p>{{ post.excerpt }}</p>
      <a class="read-more" href="{{ post.url }}">Read more...</a>
    </li>
  {% endfor %}
</ul>
