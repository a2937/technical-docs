---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Addition
layout: documentation
topic1: Overview
topic2: Pitfalls
topic3: What can you do?
------
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="overview" class="main-section">

<header>Overview</header>
<p>In most languages adding two numbers seems extremely easy.</p>
<p>Just add a plus sign between your two variables and boom; you now have the result.</p>
<p>Same thing regarding concatenation between two strings.</p>
<p>However with Javascript typing situation; it is a little more complicated then that.</p>
</section>
<br/>

<section id="pitfalls" class="main-section">

<header>Pitfalls</header>
<p>Suppose you have a plus sign between a variable
storing a string of a number and an actual number data type.</p>
<p>Which type is the actual outcome going to be?</p>
<p>The answer is that depends.</p>
<p>Javascript likes to suddenly mutate types for you if they don't match.</p>
<p>If there's a number as the left numerator; odds are in your favor
it's going to be a number.</p>
<p>Likewise if there's a string of a number of the left ; the odds are in your favor
that it will be a string.</p>
</section>
<br/>

<section id="what_can_you_do" class="main-section">

<header>What can you do?</header>
<p>So if it's going to be unreliable what can you do?</p>
<p>Beyond migrating your own project directly to Typescript;
or compiling your Javascript to static byte code (with Nwjc, a part of Node-webkit) and getting locked into a operating system; that's not a lot of giant steps you can do.</p>
<p>If you're not ready for major changes ; either look into Flow or using Typescript
definition files and Javascript Docs to provide crisp identification of what your types
are.</p>
<p>And hope you don't mislabel anything.</p>
</section>
<br/>
