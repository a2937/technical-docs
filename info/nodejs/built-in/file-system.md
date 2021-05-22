---
title: Running a web server
layout: documentation
topic1: introduction
topic2: Methods
topic3: Flags
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="introduction" class="main-section">

<header>
  <p>NodeJS fs module</p>
</header>
<p>Today we will be able to write, read, and modify files on the hard drive.</p>
<p>This is one of the ways to maintain persistent data storage.</p>
<p>Ensure NodeJS is installed on your computer and then create a new empty app by running the following command.</p>
<code>npm init</code>
<p>Fill out the relevant information an hit enter. After that there should be a package.json</p>

</section>

<section id="Methods" class="main-section">

<header>
  <p>NodeJS fs module</p>
</header>

<p>The most popular methods to use from this module include:</p>
<ul>
<li>writeFileSync</li>
<li>readFileSync</li>
<li>existsSync</li>
<li>writeFile</li>
<li>readFile</li>
<li>exists</li>
</ul>
<p>The difference between the sync methods and the regular methods
is that the synchronous methods return the value directly and also block the
the thread.</p>
<p>It is generally preferred to use asynchronous methods with a callback function; or
rely on the promises api (code executes immediately after the method finished in it's
own private function. By being asynchronous, you can run multiple functions in parallel.</p>
<p>Note:later editions of Javascript have the await/async pattern from C# available;
you can call an asynchronous method from a regular method using wait. More about this in another
section.</p>
</section>

<section id="flags" class="main-section">

<header>
  <p>NodeJS fs module</p>
</header>


</section>
