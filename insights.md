---
layout: page
title: Insights
permalink: /insights/
eyebrow: Insights
lede: "Analysis and commentary on privacy, cybersecurity, AI regulation, and technology law."
description: "Insights from Fischer Law on data privacy, cybersecurity, AI regulation, and technology law."
---

<ul class="post-list">
{%- for post in site.posts -%}
  <li>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.description | default: post.excerpt | strip_html | truncatewords: 40 }}</p>
    <a class="link-arrow" href="{{ post.url | relative_url }}">Read more {% include icon.html name="arrow" %}</a>
  </li>
{%- endfor -%}
</ul>
