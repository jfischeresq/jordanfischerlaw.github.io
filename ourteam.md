---
layout: page
title: Our Team
permalink: /ourteam/
---

<div id="team" style="display: flex; flex-direction: row; justify-content: center;">
{% for person in site.team %}
  
  <!-- Person container -->
  <div style="display: flex; flex-direction: column; align-items: center; flex-wrap: wrap; ">
      <img style="max-height:500px; margin:10px; " src="{{ person.image_path }}">
      
      <a href="{{ person.url }}">
      <h2>{{ person.name }}</h2>
      </a>
      <!-- <p>"{{ person.excerpt }}"</p> -->
  </div>
    
{% endfor %}
</div>