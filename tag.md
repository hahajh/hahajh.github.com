---
layout: default
title: Tag archive
---
<div class="page-content wc-container">
  <h1>Tag Archive</h1>  
  {% capture tags %}
  	{% for tag in site.tags %}    
  		{{ tag[0] }}
    {% endfor %}
  {% endcapture %}
  {% assign sortedtags = tags | split:' ' | sort %} 
  
  {% for tag in sortedtags %}    
    <li><a href="/blog/tag/{{ tag }}">{{ tag }}</a></li>
  {% endfor %}
</div>