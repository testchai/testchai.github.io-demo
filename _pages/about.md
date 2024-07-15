---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

[//]: # ({% if site.google_scholar_stats_use_cdn %})

[//]: # ({% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %})

[//]: # ({% else %})

[//]: # ({% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %})

[//]: # ({% endif %})

[//]: # ({% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %})

[//]: # (true，结果为：https://cdn.jsdelivr.net/gh/zychai/zychai.github.io@gs_data_shieldsio.json)

[//]: # (false，结果为 https://raw.githubusercontent.com/zychai/zychai.github.io/google-scholar-stats/gs_data_shieldsio.json)

[//]: # (后面这里可以参照masthead.html写个循环? md文件可以写循环吗？写循环会被渲染出来吗)

<!-- <span class='anchor' id='about-me'></span>

{% include_relative includes/intro.md %}

{% include_relative includes/educations.md %}

{% include_relative includes/news.md %}

{% include_relative includes/pub.md %}

{% include_relative includes/projects.md %}

{% include_relative includes/presentations.md %}

{% include_relative includes/honers.md %}

{% include_relative includes/internships.md %} -->

<!-- If you like the template of this homepage, welcome to star and fork [Yi Ren](https://github.com/RayeRen)'s open-sourced template version [AcadHomepage ![](https://img.shields.io/github/stars/RayeRen/acad-homepage.github.io?style=social)](https://github.com/RayeRen/acad-homepage.github.io). -->


{% for link in site.data.navigation.main %}
  <span class='anchor' id = link.url></span>
  {% include_relative includes/news.md %}
{% endfor %}

If you like the template of this homepage, welcome to star and fork [Yi Ren](https://github.com/RayeRen)'s open-sourced template version [AcadHomepage ![](https://img.shields.io/github/stars/RayeRen/acad-homepage.github.io?style=social)](https://github.com/RayeRen/acad-homepage.github.io).