---
layout: post
title: IDA Pro auto-offset
description: "If your 'o' key is wearing out from converting IDA immediate values into offsets, try this bit of code."
modified: 2015-8-15
tags: [IDA Pro, code, Python]
comments: false
image:
  feature: idalarge.gif
  credit: hex-rays.com
  creditlink: https://www.hex-rays.com/products/ida/
---

### Another day with IDA...

So you have IDA runnig and you dropped in some random binary that you just pulled from a black-box.  Every little bit of context helps and those strings used via immediate offsets are invaluable hints for what a section of code is up to.  Sure, you could press 'o' every time you come across an immediate that wasn't automatically treated as an offset, but wouldn't it be nice to have this done for you?  The little code snippet below may as well be the "hello world" of IDA scripting because everyone else has probably done it already.  Here is a version to share, for those of you who don't feel like doing it yourself.

{% gist aSmig/ab4324027bb13c63e9c0 %}

Please feel free to improve and submit pull requests.  (Get yourself to the GitHub Gist with the link in the bottom left of the code window.)  Thanks to @jessemichael for sending me down this path.
