---
layout: post
title: Walky Sprite
description: "Me, as a sprite, walking."
date: 2017-08-29
tags: [design, animation, gaming]
comments: false
share: false
---


Inspired by the fun I've been having playing Earthbound in the last few weeks, I decided to immortalize my likeness in these little pixels.  


So here's me, as a sprite, walking.  Try the arrow keys! 😊

<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>AJ Kueterman</title>
</head>

<div class="container">
<div id="slideshow">
    <img style="padding-top:100px;max-width:500px;display:block;margin:auto;" alt="slideshow" src="https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/aj-front-left-walking-gif.gif?raw=true" id="imgClickAndChange" onclick="showPeace()" />
</div>
</div>

<script>
    var imgs = ["https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/aj-front-left-walking-gif.gif?raw=true", "https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/aj-front-right-walking-gif.gif?raw=true", "https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/aj-front-walking-gif.gif?raw=true", "https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/aj-back-walking-gif.gif?raw=true"];
    var peace = "https://github.com/robotsquidward/robotsquidward.github.io/blob/master/images/sprite_ajk_00.png?raw=true";

    function changeImage(dir) {
        var img = document.getElementById("imgClickAndChange");
        img.src = imgs[dir];
    }

    function showPeace() {
        var img = document.getElementById("imgClickAndChange");
        img.src = peace;
    }

    document.onkeydown = function(e) {
        e = e || window.event;
        if (e.keyCode == '37') {
            changeImage(0)
        } else if (e.keyCode == '38') {
            changeImage(3)
        } else if (e.keyCode == '39') {
            changeImage(1)
        } else if (e.keyCode == '40') {
            changeImage(2)
        }
    }

</script>
