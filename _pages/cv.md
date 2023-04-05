---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Applied Mathematics with a qualification in Mathematical Methods, Universidade de São Paulo, 2024 (expected)

Resarch experience
======
* Scientific Initiation Scholarship: "Riesz basis and non-harmonic Fourier series"
  * Escola Politécnica, Universidade de São Paulo
  * Duration: April 2022 - March 2023
  * Advisor: Professor Alexandre Kawano


Research
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
