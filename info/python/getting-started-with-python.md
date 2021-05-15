---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting started with Python
layout: documentation
topic1: Getting a code editor

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Getting_an_code_editor" class="main-section">

<header>Getting an code editor</header>
<p>Before we can get started; we need to install a code editor.</p>
<p>For the inexperienced programmer; we can use the built-in IDLE editor
or PyCharm's free Community Edition (you can get the pro version for free if you are
attending an accredited University; check with the faculty for further details).</p>
</section>
<br/>
