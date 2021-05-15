---
title: JSON Files
layout: documentation
topic1: intro

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}


<section id="intro" class="main-section">

<header>
  <p>Javascript Object Notation (JSON) Files</p>
</header>

<p>The Javascript Object Notation (JSON) file is a
data file that consists of key value pairs (e.g {id:1}).</p>

<p>The format is a way to represent objects in in Javascript; if
it wasn't clear based on the name.</p>
<p>Every object must be contained in a pair of opening and closing
brackets.</p>
<p>Every key must be wrapped in double quotes(known as a string in programming and the only
way to represent words); and they must have a colon after it followed by the value.</p>
<p>After each value there must be a comma before the new key is declared.</p>
<p>Values can literally be any type.</p>
<p>Javascript objects also are capable of nesting other objects inside them as values.</p>
<p>And lastly they can store arrays (structures that are essentially a list
but the first object index starts at zero instead of one).</p>
<p>All arrays are represented by having an pair of opening and closing
braces, with the values being inside of them separated by commas.</p>

<p>Here is an example of valid JSON very concept shown.</p>
<br/>
<br/>
<code>
{
  "key1": 1,<br/>
  "parentKey": {<br/>
    "child": "value"<br/>
  },<br/>
  "array": [<br/>
    "value1",<br/>
    "value2",<br/>
    "value3" <br/>
  ]
}
</code>

<!--
TODO: Figure out what I need to elaborate on and how to break this up better.
-->

</section>
