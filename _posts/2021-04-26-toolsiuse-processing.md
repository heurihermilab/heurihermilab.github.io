---
title: "Tools I use: Processing"
excerpt_separator: "<!--more-->"
categories:
  - blog
tags: 
  - toolsiuse
  - graphics
  - video
  - programming
  - design
  - Processing
---

Tools I use: Processing



The (nearly-unGoogleable) cross-platform programming language and development system **Processing** is one of my secret weapons when it comes to graphics, especially motion graphics for video. The Java-derived language is simple, easy to share and hack, and rewards serendipity, yet hits the sweet spot in terms of pixel-level control without overwhelming with obligatory detail and system-level apparatus. 

<!--more-->

Like HyperCard, Processing has the virtue of being a simple way to get ideas on to the screen without learning the technical ins and outs of the operating system, while facilitating maximum freedom in what one can programmatically construct. Its Hello World has two functions, `setup` and `draw`, with four executable lines. Yet the programmer is free to create class and function hierarchies like any object-oriented environment. 

Libraries and extensions to the system promise even greater vistas of manipulation and control, though I must admit that aside from the library that renders MP4 files I've found the built-in capabilities engrossing/challenging enough that I've yet to explore them.

One negative aspect that's come with Processing's multi-platform success is language fragmentation, as the browser-oriented JavaScript-based variation integrates with the browser closely enough that even the drawing model is different, with no straightforward translation between it and the original version. There seems to be no documentation available about the differences, either, that could facilitate transcoding from one to the other, you simply have to learn them both.

This fragmentation also hinders learning via OpenProcessing examples, as most of the "classic" Processing sketches are now archived in favor of browser-based JavaScript versions that execute well online in browsers, natch. I don't question the maintainers' intent but it *is* a pain, and I say that as someone who's transcoded Processing into Swift.


**Tool** | Processing [[wikipedia]](https://en.wikipedia.org/wiki/Processing_(programming_language))

**What it is** | A cross-platform IDE and programming language (aka DSL) built for electronic art and design, with two main variants:
- Processing — based on Java
- Processing.js and p5.js — language targeting Web browsers based on JavaScript

Positives:
- Free
- Offers generous level of control with minimal apparatus
- Highly extensible

Negatives:
- Fragmentation of language and subsequent documentation swamp
- "Sketchbook" organizational metaphor encourages storing multiple versions of basic sketches and redundant source files

Links:
- [Processing](https://processing.org/)
- [OpenProcessing](https://openprocessing.org/)