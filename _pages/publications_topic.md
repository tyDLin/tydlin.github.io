---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics: [Generative Artificial Intelligence, Machine Learning, Optimization, Game Theory, Optimal Transport, Ph.D Thesis]
nav: false
---

<div class="publications">
{% for t in page.topics %}
  <h1 class="year">{{t}}</h1>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}
</div>
