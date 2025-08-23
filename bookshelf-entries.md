---
layout: default
title: "All Bookshelf Entries"
permalink: /bookshelf-entries/
---

# All Bookshelf Entries

Every note from the Restless Bookshelf, newest first.

<ul class="entry-list">
  {% assign entries = site.posts | sort: "date" | reverse %}
  {% for post in entries %}
    {% if post.book and post.author and post.book_url %}
      <li class="entry-item">
        <a href="{{ site.baseurl }}{{ post.book_url }}#{{ post.slug }}" class="entry-title">
          {{ post.title }}
        </a>
        <span class="entry-date">[{{ post.date | date: "%B %d, %Y" }}]</span><br>
        <span class="entry-book">{{ post.book }} — {{ post.author }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

[← Back to the Restless Bookshelf]({{ site.baseurl }}/bookshelf/)
