---
layout: page
title: 2315zhz
---

<div id="posts">
  <h2>Posts</h2>
  <ul>
    {% for post in site.posts %}
      <li style="font-size: 18pt"><a href="{{ post.url }}">{{ post.title }}</a><span style="font-size: 14pt"> - {{ post.date | date_to_string }}</span><br/><br/>
      {% assign desc = post.content | split: '</p>' %}
      <blockquote>
        {{ desc.first }} (<a href="{{ post.url }}">read more</a>)</p>
      </blockquote>
      </li>
    {% endfor %}
  </ul>
</div>

