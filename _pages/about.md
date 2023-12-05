---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<style>
  .title_local {
    font-family: "Arial Narrow"; /* Set the font family */
    font-size: 20px; /* Set the font size */
    font-weight: bold;
    color: rgb(29, 28, 27);
  }
</style>

{% include base_path %}

I am ...

<div class = "title_local"> 
  News
</div>

<div class = "title_local"> 
Publications
</div>
  <ul>
    {% for post in site.publications %}
    {% include archive-single-cv.html %}
    {% endfor %}
  </ul>

<div class = "title_local"> 
  Projects
</div>

  
<div class = "title_local"> 
  Talks
</div>

  <ul>
    {% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
    {% endfor %}
  </ul>