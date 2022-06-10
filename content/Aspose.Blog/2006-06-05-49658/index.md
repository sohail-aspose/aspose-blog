---
title: 'Aspose.Slides for Java 1.6.4.0 released!'
date: Mon, 05 Jun 2006 05:40:00 +0000
draft: false
url: /2006/06/05/49658/
author: Alcrus
summary: ''
tags: ['Alexey Zhilin']
---

Hot fix contains:  

*   New: Wrapping Eastern Langauges text. For correct work Eastern fonts should be installed.  
    
*   New: Creating shapes inside groups.
*   New: Serializing shapes to a stream and loading it back to the same or another slide or presentation. Supported shapes are Line, Rectangle, Ellipse, AutoShape, Polyline, PictureFrame. In this release OleObjectFrame, AudioFrame and VideoFrame can be serialized and restored back as PictureFrame only. GroupShape and Table can't be serialized.
*   New: Small memory optimization. We are planning to continue optimizing Aspose.Slides in the next hot fixes.
*   Fixed: PHP Presentation and Slide classes didn't close stream after writing PPT and SVG files.







