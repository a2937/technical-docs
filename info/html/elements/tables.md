---
title: Tables
layout: documentation
topic1: Overview
topic2: Example
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Overview" class="main-section">

<header>
  <p>Tables</p>
</header>
<p>Tables are the best way to display to show
off rows of records on a web page.</p>
<p>There are three main elements involved in display a table on a webpage:</p>
<ul>
<li>table - the outermost container for the table</li>
<li>tr - a row in the table</li>
<li>th - a header for the table that belongs in the first row</li>
<li>td - data for the table </li>
<ul>
</section>

<section id="Example" class="main-section">

<header>
  <p>Example</p>
</header>
<p>Here is what the markup for a simple table should look like</p>

<button class="collapsible">View Code</button>
<div class="content">
  <code>
        &lt;!DOCTYPE html&gt;<br/>
        &lt;html lang=&quot;en&quot;&gt;<br/>
        &lt;head&gt;<br />
        &lt;meta charset=&quot;UTF-8&quot;&gt;<br />
        &lt;meta http-equiv=&quot;X-UA-Compatible&quot; content=&quot;IE=edge&quot;&gt;<br />
        &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;<br />
        &lt;title&gt;Document&lt;/title&gt;<br />
        &lt;/head&gt;<br />
        &lt;body&gt;<br />
        &lt;table&gt;<br />
        &lt;tr&gt;<br />
        &lt;th&gt;<br />Column A&lt;/th&gt;<br />
        &lt;th&gt;<br />Column B&lt;/th&gt;<br />
        &lt;/tr&gt;<br />
        &lt;tr&gt;<br />
        &lt;td&gt;<br />Value A&lt;/td&gt;<br />
        &lt;td&gt;<br />Value B&lt;/td&gt;<br />
        &lt;/tr&gt;<br />
        &lt;/table&gt;<br />
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
</section>
