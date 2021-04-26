---
title: Running a web server
layout: documentation
topic1: introduction
topic2: Basic Text Element
topic3: Headings

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="introduction" class="main-section">

<header>
  <p>ExpressJS</p>
</header>
<p>Today we will be building a very bare-bones ExpressJS
server.</p>
<p>ExpressJS is a NodeJS-powered web server. It can be used to serve
documents or run an API.
<p>Ensure NodeJS is installed on your computer and then create a new empty app by running the following command.</p>
<code>npm init</code>
<p>Fill out the relevant information an hit enter. After that there should be a package.json

</section>
