---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: String Manipulation
layout: documentation
topic1: Overview
topic2: Trimming


---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<!--
TODO : Talk about strings in Ruby
-->

<section id="Trimming" class="main-section">

<header>Trimming</header>
<p>Before we can compare strings; first we need to be trim
out all the white space.</p>
<p>Otherwise despite thinking " Jack " and "Jack" seem
equal; the program won't think so.</p>
<p>The String method we are looking for is called "strip"
and will return a copy of the string you want to trim.</p>
<code>"abc".strip == " abc ".strip </code>
<p>This section of code will return true because the result
is the same.</p>
<p>However if you wish to modify the variable in-place : you have to append
an exclamation mark after it.<p>
<p>Unfortunately it will only return a value if it is modified. It would be
best to directly call it on the variable before any comparisons.</p>
<p>Like so:</p>
<code>
@myNameVariable = " Jack "
@myNameVariable.strip!
@myNameVariable == "Jack" # Should return true
</code>

</section>
<br/>
