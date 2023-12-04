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
      font-size: 25px; /* Set the font size */
      /* font-weight: bold; */
      color: rgb(61, 53, 61);
  }
  /* Style for the container */
  .container {
    display: flex;
    justify-content: space-between;
    
  }

  /* Optional: Add styling for text and date if needed */
  .text {
    font-weight: bold;
    font-family: "Arial Narrow"; /* Set the font family */
    font-size: 15px; /* Set the font size */
  }

  .date {
    color: #888;
    font-family: "Arial Narrow"; /* Set the font family */
    font-size: 15px; /* Set the font size */
  }
</style>

{% include base_path %}

<div class = "title"> 
Education
</div>
<span class="container">
  <div class="text">B.S. in Applied Mathematics, University of Dschang,</div>
  <div class="date">2012 - 2015</div><br>
</span>
<span class="container">
  <div class="text">M.S. in Applied Mathematics, University of Dschang,</div>
  <div class="date">2015 - 2017</div>
</span>
<span class="container">
  <div class="text"> M.S. in Industrial Mathematics, University of Dschang,</div>
  <div class="date">2017 - 2019</div>
</span>
<span class="container">
  <div>M.S. in Machine learning, African Masters of Machine Intelligence,</div>
  <div class="date">2019 - 2020</div>
</span>
<span class="container">
  <div class="text">Ph.D Bayesian inverse problems, Heriot-Watt University,</div>
  <div class="date">2021 - Todate</div>
</span>


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
