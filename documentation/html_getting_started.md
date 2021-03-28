---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Getting started with Javascript
layout: documentation
topic1: Getting a code editor
topic2: Hello World
topic3: Your first function
topic4: Using our first function
topic5: Script tags
---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="Getting_an_code_editor" class="main-section">

<header>Getting an code editor</header>

Before you can begin to program, first you have to install an file editor.

Older softwares love to use by Vi (a linux text editor: short for Vi) or even Notepad.

However this puts you at an unfortunate disadvantage.

There is no debug information or highlighting to indicate whether or not anything actually works.

Fortunate for us, we'll be using the Visual Studio Code editor.

Navigate to <a href="https://code.visualstudio.com/">Visual Studio's main website<a/> and get the stable build.

Click the download button and run the installer.

Click through the various options.

Open it up and you should be ready to write some code.

</section>
<br/>
<section id="Hello_World" class="main-section">

<header>Hello World</header>


<p>To start off with, we will be running code in the browser.</p>

<header>Hello World</header>
<p>To start off with, we will be running code in the browser.</p>
<p>Open Visual Studio Code to a blank document and save it as <em>index.html</em>.</p>
<p>This tells Visual Studio Code we want features related to HTML (hyper text markup language).</p>
<p>For those unaware html opening and closing tags to express elements of the page.</p>
<p>Next we'll be using an <em>Emmet</em> abbreviation to fill out a beginner html page.</p>
<p>Type the following into Visual Studio Code and hit enter.</p>
<code>html:5</code>
<p>It should fill out a page similar to below. If not adjust it to match.</p>

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
<p>We're next going to add a script tag element.</p>
<p>This element allows code to be ran on your web page.</p>
<p>Underneath the opening tag to the body, we are going to write</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
  &lt;script&gt;
      console.log("hello world");
      &lt;/script&gt;
  </code>
</div>
<br/>
<p> When our web page gets opened; it will evaluate the code inside. </p>
<p>Open your webpage in the browser and navigate to the developer tools.</p>
<p>This is typically opened by pressing the F12 key on the keyboard.</p>
<p>Once there navigate to the <em>console</em> tab on the developer tools.</p>
<p>The latest line should say <em>Hello World</em>.</p>
<p>If not, please check your document and see that it matches below</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
    &lt;!DOCTYPE html&gt;<br />
    &lt;html lang=&quot;en&quot;&gt;<br />
    &lt;head&gt;<br />
    &lt;meta charset=&quot;UTF-8&quot;&gt;<br />
    &lt;meta http-equiv=&quot;X-UA-Compatible&quot; content=&quot;IE=edge&quot;&gt;<br />
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;<br />
    &lt;title&gt;Document&lt;/title&gt;<br />
    &lt;/head&gt;<br />
    &lt;body&gt;<br />
    &lt;script&gt;console.log("Hello World");&lt;/script&gt;<br/>
    &lt;/body&gt;<br />
    &lt;/html&gt;<br />
  </code>
</div>
<br/>
<p>Pat yourselves on the back for getting this far.</p>
<p>And if necessary take a break before going onto the next section.</p>
</section>
<br/>
<br/>
<section id="Your_first_function" class="main-section">

<header>Your first function</header>
<p>Now we are going to write code in a separate file.</p>
<p>Create a new file in your directory called <em>index.js</em>.</p>
<p>This a proper Javascript file and will be used to contain our code.</p>
<p>There are a load of advantages over writing code directly on the page including but not
limited to: reuse, modularity, and convenience.
</p>
<p>Inside the file we are going to write a function that will turn our background pink.</p>
<p>A function is an executable piece of code that will perform an action.</p>
<p>We'll start by writing the function header.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
<br/>
<code>
    function turnBackgroundPink() 
</code>
<br/>
</div>
<br/>
<p>This declares we are creating a function called <em>turnBackgroundPink</em>.</p>
<p>The function keyword indicates that the following is a function.</p>
<p>And the two parenthesis are designed to hold any data passed to our function.</p>
<p>Next we will be adding a function body. Create an opening and closing curly brace after the closing
  parenthesis.
</p>
<p>Here is what it should look like so far below.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
      function turnBackgroundPink()<br/>
      {<br/>
        <br/>
      }<br/>
  </code>
</div>
<br/>
<p>Next we are going to write a line of code that will add the background-color style property to our document
  body.
</p>
<p>Here is what the line looks like below.</p>

<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
  document.body.style = "background-color:pink";
  </code>
</div>
<br/>
<p>To summarize what this does, basically the <em>document</em> property represents the current html page in
  memory.</p>
<p>Next we are locating the body element of the page that exists on the <em>document</em> object.</p>
<p>Then we are setting the style property of that element to affect the background-color, and setting it to pink.
</p>
<p>This is in JSON (JavaScript Object Notation). JSON consists of key value pairs and can have interior properties
  set with colons rather than an equal sign.
</p>
<p>More on <a href="https://www.w3schools.com/Js/js_json_objects.asp">JSON</a> here.</p>
<p>Here's what the end result should look like.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
  function turnBackgroundPink()<br/>
  {<br/>
    document.body.style = "background-color:pink";<br/>
  }<br/>
  </code>
</div>
<br/>
</section>
<br/>
<section id="Using_our_first_function" class="main-section">

<header>Using our first function</header>

<p>In the last section we defined our last function but didn't use it yet.</p>
<p>Go back to <em>index.html</em>.</p>
<p>Above the closing body tag we are going to add a new script tag.</p>
<p>This time though we are setting the src (source) attribute of the script tag.</p>
<p>The src attribute is used to literally point to a javascript source file.</p>
<p>Here is what the script tag should look like.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
    &lt;script src=&quot;index.js&quot;&gt;<br/>
    &lt;/script&gt;<br/>
  </code>
</div>
<br/>
<p>This script tag says as soon as possible put this script file into memory.</p>
<p>This is why typically all script tags go above the closing body tag; to improve website responsiveness.</p>
<p>If you open up the developer tools and go to the console, we should see turnBackgroundPink function is defined.
</p>
<p>However it isn't doing anything.</p>
<p>In the section we will be actually running it when the page loads.</p>
</section>
<br/>
<section id="Script_tags" class="main-section">

<header>Script tags</header>
<p>In the last section we finally created a function and hooked it up to our main page.</p>
<p>Now we are going to have this function execute automatically. </p>
<p>Add a new script tag below the one you just added.</p>
<p>You should have something like this.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
    &lt;!DOCTYPE html&gt;<br />
    &lt;html lang=&quot;en&quot;&gt;<br />
    &lt;head&gt;<br />
    &lt;meta charset=&quot;UTF-8&quot;&gt;<br />
    &lt;meta http-equiv=&quot;X-UA-Compatible&quot; content=&quot;IE=edge&quot;&gt;<br />
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;<br />
    &lt;title&gt;Document&lt;/title&gt;<br />
    &lt;/head&gt;<br />
    &lt;body&gt;<br />
    &lt;script src=&quot;index.js&quot;&gt;<br/>
    &lt;/script&gt;<br/>
    &lt;script&gt; <br/>
    &lt;/script&gt; <br/>
    <br/>
      &lt;/body&gt;<br />
      &lt;/html&gt;<br />
    </code>
  </div>
<br/>
<p>In the last script tag we are going to call our function.</p>
<p>In the final script tag we are going to write <em>turnBackgroundPink()</em></p>
<p>Here's what the final html page should look like.</p>
<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
    &lt;!DOCTYPE html&gt;<br/>
    &lt;html lang=&quot;en&quot;&gt;<br/>
    &lt;head&gt;<br/>
    &lt;meta charset=&quot;UTF-8&quot;&gt;<br/>
    &lt;meta http-equiv=&quot;X-UA-Compatible&quot; content=&quot;IE=edge&quot;&gt;<br/>
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;<br/>
    &lt;title&gt;Document&lt;/title&gt;<br/>
    &lt;/head&gt;<br/>
    &lt;body&gt;<br/>
    &lt;script src=&quot;index.js&quot;&gt;<br/>
    &lt;/script&gt;<br/>
    &lt;script&gt;<br/>
    turnBackgroundPink();<br/>
    &lt;/script&gt;<br/>
    &lt;/body&gt;<br/>
    &lt;/html&gt;<br/>
  </code>
</div>
<br/>
<p>The call script tag must come afterwards because every script tag is loaded sequentially (the order
in which they go down the page.)</p>

<p>
So after reading this you should have a rough understanding of how to:
</p>

<ul>
  <li>Install Visual Studio Code</li>
  <li>Use a shortcut to create a basic html5 website.</li>
  <li>Run code on a webpage.</li>
  <li>Create and reference a Javascript source file</li>
  <li>Link script tag content together.</li>
</ul>
</section>