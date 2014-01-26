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

```Haskell
evaluate :: ComonadApply f => f (f b -> b) -> f b
evaluate fs = fix $ (fs <@>) . duplicate
```

I'll be writing much more about this project very soon!
