---
layout: default
title: Blog
permalink: /blog/
order: 3
---
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>anita mehrotra</title>
    <link rel="stylesheet" href="stylesheets/styles.css">
    <link rel="stylesheet" href="stylesheets/github-light.css">
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
  </head>

<div class="body">
  <div class="inner-body">
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
</div>

</head>