---
layout: default
title: Blog
permalink: /blog/
order: 3
---

<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>avanti mehrotra</title>
    <link rel="stylesheet" href="stylesheets/styles.css">
    <link rel="stylesheet" href="stylesheets/github-light.css">
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
  </head>
</html>

<div class="body">
  <p class="quote">"People who love to eat are always the best people." ~ Julia Child</p>
  <hr class="line">
  <ul class="post-list">
    {% for post in site.posts %}
    <li class="list">
      <h4 class="date">{{ post.date | date: "%-d %B %Y" }}</h4>
      <h4 class="post-title"><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h4>
      {{ post.content | strip_html | truncatewords: 50 }}
    </li>
    {% endfor %}
  </ul>
</div>

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-80756232-1', 'auto');
  ga('send', 'pageview');

</script>