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

I am a Research Scientist at [Luma AI](https://lumalabs.ai/dream-machine). I am also a Ph.D. student (on leave) at Stanford University advised by [Prof. Stefano Ermon](https://cs.stanford.edu/~ermon/). I previously received my bachelor's degrees in Computer Science and Applied
Mathematics at University of California, Los Angeles and was advised by [Prof. Song-Chun Zhu](http://www.stat.ucla.edu/~sczhu/) and [Prof. Ying-Nian Wu](http://www.stat.ucla.edu/~ywu/me.html). 
I work on machine learning methods for generative modeling.

I was a co-founder at [Apparate Labs](https://apparate.ai/index.html) (acquired by [Luma AI](https://lumalabs.ai/dream-machine)) focusing on real-time visual synthesis of human-centric videos. 


<br>

<h1 id="publications"> Publications</h1>

<hr style="width:80%;text-align:left;margin-left:0">

{% for post in site.publications reversed %}
  {% include archive-single-pub.html %}
{% endfor %}