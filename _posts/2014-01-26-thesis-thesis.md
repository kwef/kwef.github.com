---
layout: post
title: "Thesis? Thesis!"
description: ""
category: code
tags: []
---
{% include JB/setup %}

Yesterday I spoke with my wonderful advisor, and I spent about two hours talking with him about this idea I've been working on. It's to do with infinite multidimensional spreadsheets in Haskell, and I've already [got some of it up and running](https://github.com/kwef/ZipperSheets). And so, with that, I have a senior thesis topic! I'm overflowing with excitement.

Here's a sneak preview of the neato fixed-point operator that forms the heart of the whole operation:

{% gist 8636894 %}

You can use it to succinctly define the infinite [Pascal's triangle](http://en.wikipedia.org/wiki/Pascal's_triangle)...

{% gist 8636921 %}

...and then get out a finite chunk of it:

{% gist 8637051 %}

There's a lot more to this project, and rest assured, I'll be writing much more about it soon!
