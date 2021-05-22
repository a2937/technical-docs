---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Videos
layout: documentation
topic1: Overview
topic2: Controlling videos
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Overview" class="main-section">

<header>
  <p>Videos</p>
</header>
<p>In modern html5 there are fully functional video components.</p>
<p>To the best of the knowledge of the author a video file
is just a bunch of pictures layered on top of each other.</p>
<p>However that being said
<p>This will be our starting document. </p>

<br/>
<br/>
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
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
</section>



<section id="controlling_videos" class="main-section">
<!--
Todo : Talk about the start method to begin a video
and the pause method to stop a video
-->
</section>
