---
layout: page
title: Blog
include_in_header: true
include_in_footer: true
---

# Blog

Explore evidence-based strategies for happiness, well-being, and personal growth.

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% assign valid_posts = "" | split: "" %}
{% for post in sorted_posts %}
  {% if post.title and post.title != "" %}
    {% assign valid_posts = valid_posts | push: post %}
  {% endif %}
{% endfor %}

{% for post in valid_posts limit:1 %}
<div class="blog-hero">
  <h3><a href="{{ post.url | relative_url }}" target="_self">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</div>
{% endfor %}

<div class="blog-secondary">
{% for post in valid_posts limit:2 offset:1 %}
<div class="blog-secondary-card">
  <h3><a href="{{ post.url | relative_url }}" target="_self">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</div>
{% endfor %}
</div>

<h2 class="blog-section-title">More Articles</h2>

<div class="blog-posts">
{% for post in valid_posts offset:3 %}
<div class="blog-post-preview">
  <h3><a href="{{ post.url | relative_url }}" target="_self">{{ post.title }}</a></h3>
</div>
{% endfor %}
</div>
