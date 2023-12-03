---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
<style>
  .title {
    font-family: "Arial Narrow"; /* Set the font family */
      font-size: 20px; /* Set the font size */
      /* font-weight: bold; */
      color: rgb(127, 71, 127);
  }
</style>

{% include base_path %}

<div class = "title"> 
Education
</div>

* B.S. in Applied Mathematics, University of Dschang, 2015
* M.S. in Applied Mathematics, University of Dschang, 2017
* M.S. in Industrial Mathematics, University of Dschang, 2019
* M.S. in Machine learning, African Masters of Machine Intelligence, 2020
* Ph.D Bayesian inverse problems, Heriot-Watt University, 2024 (expected)

<div class = "title"> 
Work experience
</div>

* Summer 2015: Research Assistant
  * Github University
  * Duties included: Tagging issues
  * Supervisor: Professor Git

* Fall 2015: Research Assistant
  * Github University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub

<div class = "title">  
  Skills
</div>

* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

<div class = "title">
Publications
</div>

  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

<div class = "title">  
Talks
</div>

  <ul>
    {% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
    {% endfor %}
  </ul>

<div class = "title">
Teaching
</div>

  <ul>
    {% for post in site.teaching %}
    {% include archive-single-cv.html %}
    {% endfor %}
  </ul>

<div class = "title">  
Service and leadership
</div>

* Currently signed in to 43 different slack teams
