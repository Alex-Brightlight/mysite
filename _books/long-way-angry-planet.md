---
layout: default
title: "The Long Way to a Small, Angry Planet"
---

# ***The Long Way to a Small, Angry Planet*** — Becky Chambers

{% assign entries = site.posts | where:"book","The Long Way to a Small, Angry Planet" | sort: "date" %}
{% for post in entries %}
  <h2 id="{{ post.slug }}">
    {{ post.title }} <span class="post-date">[{{ post.date | date: "%B %d, %Y" }}]</span>
  </h2>
  {{ post.content }}
{% endfor %}

---

[← Back to the Restless Bookshelf]({{ site.baseurl }}/bookshelf/)

