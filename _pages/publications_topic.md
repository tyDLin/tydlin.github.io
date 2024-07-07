---
layout: page
permalink: /publications_topic/
title: Publications (by Topic)
topics_thesis: [thesis]
topics_batchRL: [continuous state-action space, policy evaluation, off-line reinforcement learning]
topics_MTL: [multi-task learning]
topics_aggreg: [state aggregation, state embedding]
nav: false
---

<div class="publications">

<h1>Ph.D Thesis</h1>

{% bibliography -f papers -q @*[topic={{thesis}}]* %}

</div>
