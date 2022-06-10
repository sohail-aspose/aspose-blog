---
title: 'SmartArt Rendering and Tight/Through Wrapping Support in Aspose.Words 11.11.0'
date: Sun, 30 Dec 2012 12:20:09 +0000
draft: false
url: /2012/12/30/smartart-rendering-and-tightthrough-wrapping-support-in-aspose.words-11.11.0/
author: Adam Skelton
summary: ''
tags: ['PDF', 'SmartArt', 'Through', 'Tight', 'Word', 'Wrapping', 'rendering']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_logo.png" alt="">}}


We are pleased to announce the release of this month’s version of Aspose.Words for .NET and Java. This release contains 161 improvements to Aspose.Words.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.11.0][1]
*   [Aspose.Words for Java 11.11.0][2]

## Partial Support for Rendering SmartArt in Word Documents

SmartArt is a feature first introduced in Microsoft Office 2007. It was designed to create simple and effective diagrams, organization charts or flow charts with many more options than previous versions of Microsoft Word.  The image below demonstrates a typical SmartArt object that you may find in a Word document:



{{< figure align=center src="images/image_4-300x295.png" alt="A SmartArt image in a word document">}}


Aspose.Words now partially renders these objects to fixed page formats such as PDF, XPS, image, etc. The introduction of this feature is a big step forward as the underlying format of SmartArt is very complex and is not a trivial task to implement rendering of these objects.

As always, keep an eye on this feature as we will be continually improving the rendering of this feature in future releases.

## Rendering Tight and Through Wrapping is now Supported

We are happy to announce that with support of both Tight and Through wrapping types, Aspose.Words now supports all wrapping types when rendering to fixed page formats. Both tight and through wrap types aren't that common and are the hardest to implement therefore they were the last to be supported.

Aspose.Words now reads and interprets the polygon wrapping points for images which are the basis of what makes tight or through wrapped images to be positioned very tightly against the text. The result when converting using Aspose.Words is text wrapping that is rendered identical to how Microsoft Word renders it:

**A sample document demonstrating tight wrapping**



{{< figure align=center src="images/TightWrapping.jpg" alt="Tight Wrapping Word Document">}}





[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




