---
title: Getting a connection with Socket.io
layout: documentation
topic1: introduction
topic2: Getting the message

---
{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<section id="introduction" class="main-section">

<header>
  <p>Socket-IO</p>
</header>
<p>Today we will be hooking up Socket.IO.</p>
<p>It's essentially a wrapper around web-sockets.</p>
<p>In order to get started; we'll need a working ExpressJS server.</p>
<p>Initialize a new project and setup an barebones ExpressJS server.</p>
<p>After that run the following command</p>
<code>npm install --save socketio</code>
<p>This will install the socketio framework to the current project.</p>
<p>After that modify the entry point to the application (either index.js or app.js
if you are using standard conventions) to load up the socket.io module.</p>
<p>After that below where you initialize the expressjs server; create an input
output instance listening on the http server.</p>
<p>In layman terms we are going to create a variable to hold the socket.io server.</p>
<p>It should look something like this.</p>
<code>const io = socket.listen(server)</code>
<p>After that is where we start creating our event emitters.</p>
<p>The very first one we want to create is an event emitter for a server
connection.</p>
<p>Below where you created the io instance write an event listener for the
connection instance with a callback function (with a socket as a parameter).</p>
<p>It should look something like this</p>
<code>
io.on('connection', function (socket) {
  console.log("Connected successfully to the socket ...");
  console.log('A user connected');
});
</code>
<p>Now whenever anyone connects to our server using socket-io, our
server will log that they connected.</p>
</section>

<section id="Getting_the_message" class="main-section">
<p>In order to actually get that message; the client has to have a SocketIO
client library loaded. Wrappers for popular programming languages exists.</p>
<p>They need to create a new socket-io instance with the address and Socket-IO port of
the server ; listen for a connection event
and get their id.</p>
<p>Each event the server emits typically needs to be listened to by the client.</p>
<p>However the socket itself can emit its own events for the server to listen to.</p>
<p>An easy way to demonstrate this is to use the public index.html that came with the ExpressJS project.</p>
</section>
