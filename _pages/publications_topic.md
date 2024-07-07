---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics: [Ph.D Thesis, Optimization and Game Theory, Machine Learning, Optimal Transport, Alternating Direction Method of Multiplier]
nav: false
---

<div class="publications">

{% for t in page.topics %}
  <h2 class="topic">{{t}}</h2>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}

</div>
