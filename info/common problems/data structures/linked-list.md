---
title: Linked Lists in a nutshell
layout: documentation
topic1: Intro
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}


<section id="intro" class="main-section">

<header>
  <p>What is a Linked List?</p>
</header>
<p>A Linked List is one of the most unique data structures out there.</p>
<p>Rather than just have every element be stored one after the other;
each element is a node that points to the next which points to the next and so on.</p>
<p>The first element is called the head; because that's where all the other elements branch off of.</p>
<p>Element1 (Head) -> Element2 -> Element3...</p>
<p>But adding nodes directly is unfortunately a security risk as well as more information
than the consumer of the class needs to know.</p>
<p>All the consumers should be able to pass in are at most an index and whatever they want to store.</p>
<p>However indexes technically don't exist on Linked Lists so take that bit with a grain of salt.</p>
</section>
