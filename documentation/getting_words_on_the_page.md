---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting words on the page
layout: documentation
topic1: Prepping
topic2: Basic Text Element
topic3: Headings

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="prepping" class="main-section">

<header>
  <p>Basic text element</p>
</header>
<p>Today we will be going over how to add text to your</p>
<p>website. There are several different available tags but</p>
<p>I will be going over the most popular text-related ones.</p>

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
<br/>
<section id="basic_text_element" class="main-section">

<header>
  <p>Basic Text element</p>
</header>

<p>All visual elements appear in the body of the html 
document.</p>

<p>The standard tag for text is the <em>p</em> tag.</p>

<p>It is called a paragraph tag and is one of the many
small building blocks of a page. </p>

<p>We will write the phrase "Hello World" on a page.</p>

<p>Underneath the opening body tag, creating an opening and closing
p tag.</p>

<p>Inside the two tags, write the phrase hello world.</p>

<p>It should look something like this. </p>
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
        &lt;p&gt;<br /> 
        hello world
        &lt;/p&gt;<br /> 
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
</section>
<br/>
<br/>
<section id="headings" class="main-section">

<header>
  <p>Headings</p>
</header>
<p>One of the first few things we can do on our page is add 
a proper title.</p>
<p>In the head section, we can change our current title <em>Document</em>
to whatever you want.</p>
<p>For the purposes of this lesson , it will be <em>My First Website</em>.</p>
<p>Scroll to the top of the document in your html editor and inside the title tag,
replace <em>Document</em> with <em>My First Website</em>.
<p>Here is how the end result should look.</p>
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
        &lt;title&gt;My First Website&lt;/title&gt;<br />
        &lt;/head&gt;<br />
        &lt;body&gt;<br /> 
        &lt;p&gt;<br /> 
        hello world
        &lt;/p&gt;<br /> 
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
</section>
<br/>
<br/>
<p>Open it in Chrome or FireFox and you should notice the tab title has changed.</p>
<p>Let's next put a title element on the page body itself.</p>
<p>Right below the body element create an opening and closing h1 tag.</p>
<p>Inside of it we will be writing the phrase <em>My First Website</em>.</p>
<p>The h1 tag represents the title as if you were editing a standard word document.</p>
<p>It is essentially heading one, and there are several subheading elements.</p>
<p>h1 up to h6 are valid html heading tags, but it should provide plenty of ways to organize
your document sections.</p>
<p>Down below is how your html page should look so far, complete with the h1 element.</p>
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
        &lt;title&gt;My First Website&lt;/title&gt;<br />
        &lt;/head&gt;<br />
        &lt;body&gt;<br /> 
        &lt;h1&gt;<br /> 
        My First Website
        &lt;/h1&gt;<br /> 
        &lt;p&gt;<br /> 
        hello world
        &lt;/p&gt;<br /> 
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
<p>So after reading this you should have a rough understanding:</p>

<ul>
  <li>How to add text to a page properly</li>
  <li>How to change the website title</li>
  <li>How to create headings on an html document</li>
</ul>
</section>