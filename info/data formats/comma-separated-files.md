---
title: CSV Files
layout: documentation
topic1: intro

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}


<section id="intro" class="main-section">

<header>
  <p>Comma Separated Value (CSV) Files</p>
</header>

<p>The Comma Separated Value (CSV) file is essentially
a text file where commas are used to separate the data.</p>

<p>Typically every the first line contains the headers and the
each line after that contains a record.</p>

<!--
TODO: Figure out what I need to elaborate on.
-->

</section>
