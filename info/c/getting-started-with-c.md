---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting started with C
layout: documentation
topic1: Getting a code editor

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Getting_an_code_editor" class="main-section">

<header>Getting an code editor</header>
<p>Before we can get started; we need to install a code editor.</p>
<p>For the inexperienced programmer; CodeBlocks is recommended since certain editions
come with setup for everything to compile and run code.</p>
<p>However for more advanced user; installing Visual Studio (or Visual Studio Code) or Eclipse is
perfectly acceptable.</p>
</section>
<br/>
