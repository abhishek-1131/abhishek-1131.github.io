---
layout: page
title: Home
---
<!--adapted from https://github.com/tameemsafi/typewriterjs You got it.-->
<div id="app" style="height:150px;"></div>
<style type="text/css">
@import url('https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap');
#app {
  font-size: 30px;
  line-height: 50px;
  font-weight: 400;
  font-family: 'Roboto', sans-serif;
}
strong {
  font-weight: 700;
}
</style>
<script src="https://unpkg.com/typewriter-effect@latest/dist/core.js"></script>
<script type="text/javascript">
var app = document.getElementById('app');
var typewriter = new Typewriter(app, { loop: true, delay: 68, });
typewriter
  .pauseFor(1000)
  .typeString('cat <strong> /var/log/life </strong>')
  .typeString('<br/>')
  .pauseFor(1000)
  .typeString('<strong> <span style="color: #27ae60;">Data | Code | Networks | Math</span> </strong>')
  .pauseFor(1800)
  .deleteChars(30)
  .typeString('<strong> <span style="color: #0096FF;">Guitar | Music Theory</span></strong>')
  .pauseFor(1800)
  .deleteChars(22)
  .typeString('<strong> <span style="color: #cb4154;">Unix | Nvim</span></strong>')
  .pauseFor(1500)
  .start();
</script>

Incoming MSc Computing Science student at [SFU](https://www.sfu.ca/computing.html). I'm primarily interested in modeling contagion spread using (location-aware) Network Graphs, Machine Learning and Topological Data Analysis. -----------
Outside work, I spend my time [reading](https://abhishek-1131.github.io/bookshelf) and playing the [guitar](https://abhishek-1131.github.io/music).
## Updates

<ul>
{% for item in site.data.updates_archive.updates limit:5 %}
<li>{{item}}</li>
{% endfor %}
</ul>
<p style="text-align:right"><a href="/newsarchive">for more news...</a></p>
