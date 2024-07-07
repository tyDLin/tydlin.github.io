---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics_thesis: [thesis]
topics_opt_game: [Variational inequality and inclusion, Equilibrium computation, Minimax optimization, Nonconvex nonsmooth optimization, High-order optimization, Alternating direction method of multiplier (ADMM)]
topics_ml: [Optimal transport, Stochastic gradient-based learning, Text analytics, Online learning]
nav: false
---

<div class="publications">

<h1>Ph.D Thesis</h1>

{% for t in page.topics_thesis %}
  <h2 class="topic"></h2>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}

<h1>Optimization and Game Theory</h1>

{% for t in page.topics_opt_game %}
  <h2 class="topic">{{t}}</h2>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}

<h1>Machine Learning</h1>

{% for t in page.topics_ml %}
  <h2 class="topic">{{t}}</h2>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}

</div>
