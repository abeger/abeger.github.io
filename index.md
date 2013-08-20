---
layout: page
title: Andy Has a Blog
tagline: Posting for the future today
---
{% include JB/setup %}

{% for post in site.posts %}
  <article>
    <h4>
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </h4>
    {{ post.content }}
    <p class="meta">
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.date | date_to_long_string }} </a>
    </p>
  </article>
  <hr />
{% endfor %}
