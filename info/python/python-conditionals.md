---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting started with Python
layout: documentation
topic1: Decisions

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Decisions" class="main-section">

<header>Decisions</header>
<!--
It would be awesome to have a little snake facing
a fork in  the road here
-->
<p>Our programs need to react to user input
and respond accordingly. That is where conditional statements come in.</p>
<p>
There are three different straight-forward operators for conditionals: the <b>if</b> statement ,
the <b>elif</b> (known as else if in other programming languages) and the <b>else</b> statement.
</p>

</section>
<br/>
