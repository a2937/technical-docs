---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Making a list
layout: documentation
topic1: Prepping
topic2: Hyperlinks

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="prepping" class="main-section">

<header>
  <p>Making a list</p>
</header>
<p>Today we will be going over how to add navigation</p>
<p>across your web pages</p>

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
<section id="hyperlinks" class="main-section">

<header>
  <p>HyperLinks</p>
</header>

<p>Hyperlinks for those are unaware is specially</p>

<p>formatted text that when you click it, you get </p>

<p>redirected to another resource.</p>

<p>We will be creating a hyperlink to the FreeCodeCamp website now.</p>

<p>To get started in the body portion of the document; create an opening and closing <em>a</em> tag.</p>

<p>Inside the two tags, write whatever you want: id</p>

<p>In the opening <em>a</em> tag add a space after the <em>a</em> write the phrase href.</p>
<p>The a stands for anchor</p>
<p><em>href</em> is a property that exists on link elements that contains the url.</p>
<p>After the href add an equal sign and a set of quotes and inside type "https://www.freecodecamp.org/"</p>
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
        &lt;a href="https://www.freecodecamp.org/"&gt;&lt;/a"&gt;<br />
        &lt;/p&gt;<br />
        &lt;/body&gt;<br />
        &lt;/html&gt;<br />
  </code>
</div>
<br/>
<br/>
<p>The href contains the link information. There are a few other types of links it can handle;
such as telephone numbers and creating emails.</p>
<p>There are two other important attributes: rel and target.</p>
<ul>
 <li>rel: determines the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Link_types">type of link</a> it is.</li>
  <li>target: determines which tab to open the link in. By default it is set to <em>_self</em></li>
</ul>
<p>A link on where to <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a">read more about anchors.</a>
<p>Note the <em>link</em> element is practically the same as an anchor element except it is used for invisible elements.
  The most common use case is setting the stylesheet and setting the rel value to <em>stylesheet</em>
  </p>
</section>

<br/>
<br/>
