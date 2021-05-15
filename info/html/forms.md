---
title: Form submissions
layout: documentation
topic1: Intro
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}


<section id="intro" class="main-section">

<header>
  <p>Forms</p>
</header>
<p>Form submissions are one of the more advanced things to do in plain html.</p>
<p>When you hit the submit button on a form; it takes your responses and sends them to an API somewhere typically.</p>
<p>And then a redirect occurs.</p>
</section>
