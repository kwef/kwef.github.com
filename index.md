---
layout: page
title: Home
---

<div id="posts">
  <h2>Recent Posts</h2><br/>
  <ul style="list-style-type: none; padding:0; margin:0">
    {% for post in site.posts limit:10 %}
      <li style="font-size: 18pt"><a href="{{ post.url }}">{{ post.title }}</a><span style="font-size: 12pt"> - {{ post.date | date_to_string }}</span><br/><br/>
      {% assign desc = post.content | split: '</p>' %}
      {% assign paragraphs = desc | size %}
      <blockquote>
        {{ desc.first }}{% if paragraphs > 1 %}<span>...</span> (<a href="{{ post.url }}">read more</a>){% endif %}</p>
      </blockquote>
      </li>
    {% endfor %}
  </ul>
  <p style="font-size: 14pt">Go to <a href="/archive.html">the full archive</a> of all {{ site.posts | size }} posts.</p>
</div>

