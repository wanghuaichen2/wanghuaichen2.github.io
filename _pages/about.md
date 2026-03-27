---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'>王怀辰</span>

{% include_relative includes/introduction.md %}

{% include_relative includes/news.md %}

{% include_relative includes/publications.md %}

{% include_relative includes/project.md %}

{% include_relative includes/honors.md %}

{% include_relative includes/educations.md %}

{% include_relative includes/internships.md %}