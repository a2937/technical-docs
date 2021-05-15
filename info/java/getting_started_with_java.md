---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting started with Java
layout: documentation
topic1: Getting setup

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Getting_setup" class="main-section">

<header>Getting setup</header>
<p>Developing programs in the Java programming language
has a few pre-requisites.</p>
<p>Warning: Before we get started this is for developing <b>desktop</b> applications
primarily and not used for adding functionality to web pages.</p>
<p>If you were looking for that, please see a tutorial related to JavaScript,
who only has in common the name elements.</p>
</section>
<br/>
