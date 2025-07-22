---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics: [Ph.D Thesis, Generative Artificial Intelligence, Game Theory, Optimization for Machine Learning, Optimal Transport]
nav: false
---

<div class="publications">
{% for t in page.topics %}
  <h1 class="year">{{t}}</h1>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}
</div>
