---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /home/
  - /home.html
  - /linqizhou
layout: archive
--- 

<hr style="width:80%;text-align:left;margin-left:0">

I am a Ph.D. student at Stanford University advised by [Prof. Stefano Ermon](https://cs.stanford.edu/~ermon/). I previously received my bachelor's degrees in Computer Science and Applied
Mathematics at University of California, Los Angeles and was advised by [Prof. Song-Chun Zhu](http://www.stat.ucla.edu/~sczhu/) and [Prof. Ying-Nian Wu](http://www.stat.ucla.edu/~ywu/me.html). 
My goal is to create human-centered embodied agents that can understand the world like humans do. Towards this end, I mainly research in computer vision and machine learning, and build models that understand the world in a structured and probablistic manner. I am
broadly interested in generative modeling and representation learning, both in unimodal and multimodal settings.

I am currently a co-founder at [Apparate Labs](https://apparate.ai/index.html), and our mission is to build real-time visual embodiment of multimodal intelligence via [generative humans](https://apparate.ai/blog/proteus.html).


<br>

<h1 id="publications"> Publications</h1>

<hr style="width:80%;text-align:left;margin-left:0">

{% for post in site.publications reversed %}
  {% include archive-single-pub.html %}
{% endfor %}