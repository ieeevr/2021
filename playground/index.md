---
layout: ieeevr-default
title: "Program Overview"
---

<h1>Data:</h1>

<ul>
{% for date in site.data.Publication %}
  <li>{{ date.Name" }}-{{ date.Published }}</li>
{% endfor %}
</ul>



<p>End data</p>
