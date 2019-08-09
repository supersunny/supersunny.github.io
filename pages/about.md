---
layout: page
title: About
permalink: /about/
weight: 1
---

# **About Me**

Welcom! My name is **{{ site.author.name }}**,<br>
I am a Graduate Student studying Computer Science. My research interest is in Machine Learning, Software Engineering, Computer vision. And in my personal life, I usually play guitar and watch movies. If you are interested in my experiences, check out other sections as well. Thank you!

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>