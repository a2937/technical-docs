---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Programming
layout: documentation
topic1: What is programming
topic2: Pseudocode
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="What_is_programming" class="main-section">

<header>What is programming?</header>

<p>All programs in their base form is a
list of instructions to follow by the computer.</p>

<p>They get an input; perform an action, and then return an output.</p>

<br/>
<br/>


<section id="Pseudocode" class="main-section">

<header>Pseudocode</header>

<p>Pseudocode in a literal definition of the word is
fake code.</p>

<p>It is used to represent our solution before we begin
programming.</p>

<p>There are multiple ways to run to write it; the easiest
way to visual it is with a flow chart. </p>
