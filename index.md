---
layout: default
title: Home
---

# Recent Posts

{% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <div class="post-meta">{{ post.date | date: "%B %d, %Y" }}</div>
    <div class="entry">
      {{ post.excerpt }}
    </div>
    <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
  </article>
{% endfor %}
