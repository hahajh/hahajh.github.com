---
layout: default
title: Tag archive
---
<div class="page-content wc-container">
  <h1>Tag Archive</h1>   
  {% for tag in site.tags %}    
    <li><a href="/blog/tag/{{ tag[0] }}">{{ tag[0] }}</a></li>
  {% endfor %}
</div>