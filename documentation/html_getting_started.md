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


To start off with, we will be running code in the browser.

Open Visual Studio Code to a blank document and save it as <em>index.html</em>.

This tells Visual Studio Code we want features related to HTML (hyper text markup language).

For those unaware html opening and closing tags to express elements of the page.

Next we'll be using an <em>Emmet</em> abbreviation to fill out a beginner html page.

Type the following into Visual Studio Code and hit enter.

`html:5`

It should fill out a page similar to below. If not adjust it to match.
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
We're next going to add a script tag element.

This element allows code to be ran on your web page.

Underneath the opening tag to the body, we are going to write
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
When our web page gets opened; it will evaluate the code inside.

Open your webpage in the browser and navigate to the developer tools.

This is typically opened by pressing the F12 key on the keyboard.

Once there navigate to the <em>console</em> tab on the developer tools.

The latest line should say <em>Hello World</em>.

If not, please check your document and see that it matches below
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
Pat yourselves on the back for getting this far.

And if necessary take a break before going onto the next section.

</section>
<br/>
<br/>
<section id="Your_first_function" class="main-section">

<header>Your first function</header>

Now we are going to write code in a separate file.

Create a new file in your directory called <em>index.js</em>.

This a proper Javascript file and will be used to contain our code.

There are a load of advantages over writing code directly on the page including but not limited to: reuse, modularity, and convenience.

Inside the file we are going to write a function that will turn our background pink.

A function is an executable piece of code that will perform an action.

We'll start by writing the function header.
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
This declares we are creating a function called <em>turnBackgroundPink</em>.

The function keyword indicates that the following is a function.

And the two parenthesis are designed to hold any data passed to our function.

Next we will be adding a function body. Create an opening and closing curly brace after the closing parenthesis.

Here is what it should look like so far below.
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
Next we are going to write a line of code that will add the background-color style property to our document body.

Here is what the line looks like below.

<br/>
<br/>
<button class="collapsible">View Code</button>
<div class="content">
  <code>
  document.body.style = "background-color:pink";
  </code>
</div>
<br/>
To summarize what this does, basically the <em>document</em> property represents the current html page in memory.

Next we are locating the body element of the page that exists on the <em>document</em> object.

Then we are setting the style property of that element to affect the background-color, and setting it to pink.

This is in JSON (JavaScript Object Notation). JSON consists of key value pairs and can have interior properties set with colons rather than an equal sign.

More on <a href="https://www.w3schools.com/Js/js_json_objects.asp">JSON</a>here.

Here's what the end result should look like.
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

In the last section we defined our last function but didn't use it yet.

Go back to <em>index.html</em>.

Above the closing body tag we are going to add a new script tag.

This time though we are setting the src (source) attribute of the script tag.

The src attribute is used to literally point to a javascript source file.

Here is what the script tag should look like.
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
This script tag says as soon as possible put this script file into memory.

This is why typically all script tags go above the closing body tag; to improve website responsiveness.

If you open up the developer tools and go to the console, we should see turnBackgroundPink function is defined.

However it isn't doing anything.

In the section we will be actually running it when the page loads.

</section>
<br/>
<section id="Script_tags" class="main-section">

<header>Script tags</header>

In the last section we finally created a function and hooked it up to our main page.

Now we are going to have this function execute automatically.

Add a new script tag below the one you just added.

You should have something like this.
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
In the last script tag we are going to call our function.

In the final script tag we are going to write <em>turnBackgroundPink()</em>

Here's what the final html page should look like.
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
The call script tag must come afterwards because every script tag is loaded sequentially (the order in which they go down the page.)

So after reading this you should have a rough understanding:

<ul>
  <li>How to install Visual Studio Code</li>
  <li>A shortcut to create a basic html5 website.</li>
  <li>How to run code on a webpage.</li>
  <li>How to create and reference a Javascript source file</li>
  <li>How to link script tag content together.</li>
</ul>
</section>