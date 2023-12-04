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
      font-weight: bold;
      color: rgb(61, 53, 61);
  }
  /* Style for the container */
  .container {
    display: flex;
    justify-content: space-between;
    
  }

  /* Optional: Add styling for text and date if needed */
  .text {
    /* font-weight: bold; */
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
<div class="container">
  <div class="text">Ph.D Bayesian inverse problems, Heriot-Watt University,</div>
  <div class="date">2021 - Todate</div>
</div>
<div class="container">
  <div class="text">M.S. in Machine learning, African Masters of Machine Intelligence,</div>
  <div class="date">2019 - 2020</div>
</div>
<div class="container">
  <div class="text"> M.S. in Industrial Mathematics, University of Dschang,</div>
  <div class="date">2017 - 2019</div>
</div>
<div class="container">
  <div class="text">M.S. in Applied Mathematics, University of Dschang,</div>
  <div class="date">2015 - 2017</div>
</div>
</div>
<div class="container">
  <div class="text">B.S. in Applied Mathematics, University of Dschang,</div>
  <div class="date">2012 - 2015</div>
</div>
<!-- sparator -->
<div class = "title"> 
Work experience
</div>
<div class="container">
  <div class="text">Teaching assistant, Heriot-Watt University,</div>
  <div class="date">2021 - 2023</div>
</div>
<div class="container">
  <div class="text">Internship, Chambre des Commerces, Cameroon</div>
  <div class="date">Jun. - Nov. 2018</div>
</div>
<!-- sparator -->
<div class = "title">  
  Skills and Certificates
</div>
<div>
  <div class="container">
    <div class="text">Design thinking, Microsoft,</div>
    <div class="date">2020</div>
  </div>
  <div class="container">
    <div class="text">Deep learning, Coursera</div>
    <div class="date">2023</div>
  </div>
</div>
<!-- sparator -->
<div class = "title">
Publications
</div>
<div>
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
    {% endfor %}
  </ul>
</div>
<!-- sparator -->
<div class = "title">  
Talks
</div>
<div>
  <ul>
    {% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
    {% endfor %}
  </ul>
</div>
<!-- sparator -->
<div class = "title">
Teaching
</div>
<div>
  <ul>
    {% for post in site.teaching %}
    {% include archive-single-cv.html %}
    {% endfor %}
  </ul>
</div>
<!-- sparator -->
<div class = "title">  
Service and leadership
</div>
* Currently signed in to 43 different slack teams
