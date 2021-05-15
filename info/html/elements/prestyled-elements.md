---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Videos
layout: documentation
topic1: Overview

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Overview" class="main-section">

<header>
  <p>PreStylized Elements</p>
</header>
<p>In modern html5 there are a handful of components that set
special display properties for you.</p>
<p>Here is a table for you</p>
<table>
 <tr>
    <th>Tag symbol</th>
    <th>Effect</th>
  </tr>
  <tr>
    <td>b</td>
    <td>Bolds text</td>
  </tr>
</table>

</section>
