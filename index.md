---
layout: page
title: You\'re doing it wrong
tagline: oh hai
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
   {% unless post.draft %}
    <li><span>{{ post.date | date_to_string }}</span> <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
   {% endunless %}
  {% endfor %}
</ul>
