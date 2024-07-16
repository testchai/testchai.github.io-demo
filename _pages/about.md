---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<!-- 要么放介绍后面，要么写到_layouts/default.html文件的页脚，或者放到about-me里。放内容最后真的不好看 -->
{% for link in site.data.navigation.main %}
  
  {% assign url_length = link.url | size %}
  
  {% assign stripped_url = link.url | slice: 3, url_length %}
  
  {% assign md_file = stripped_url | append: ".md" %}
  
  {% include_relative includes/{{md_file}} %}

{% endfor %}