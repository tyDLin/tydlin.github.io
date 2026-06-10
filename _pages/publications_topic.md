---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics: [Ph.D Thesis, Generative Artificial Intelligence, Optimization, Game Theory, Optimal Transport, Text Mining]
nav: false
---

<div class="publications">
{% for t in page.topics %}
  <h1 class="year">{{t}}</h1>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}
</div>
