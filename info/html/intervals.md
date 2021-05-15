---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Intervals
layout: documentation
topic1: Basics

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="basics" class="main-section">

<header>
  <p>Intervals</p>
</header>
<p>They are sections of code that execute very x milliseconds, where x is greater than 10.</p>

<code>setInterval(function(){ alert("Hello"); }, 3000);</code>

<p>The only way to get to stop is to call clearInterval.</p>
<code>clearInterval()</code>
</section>
