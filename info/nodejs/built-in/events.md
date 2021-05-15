---
title: Events and the Event Emitter
layout: documentation
topic1: introduction
topic2: Basic Text Element
topic3: Headings

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="introduction" class="main-section">

<header>
  <p>Events and the Event Emitter</p>
</header>
<p>Today we will be able to write, read, and modify files on the hard drive.</p>
<p>This is one of the ways to maintain persistent data storage.</p>
<p>Ensure NodeJS is installed on your computer and then create a new empty app by running the following command.</p>
<code>npm init</code>
<p>Fill out the relevant information an hit enter. After that there should be a package.json</p>

</section>


<!--

Make a reference that on some times you will have to set
chmod files because the location on the hard drive does not
have the requires permissions and the read and subsequent replaces
will fail.

-->
