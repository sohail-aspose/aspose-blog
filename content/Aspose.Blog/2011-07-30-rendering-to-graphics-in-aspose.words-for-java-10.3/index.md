---
title: 'Render Word Document Pages to PNG, BMP and JPEG in Java'
date: Sat, 30 Jul 2011 08:16:28 +0000
draft: false
url: /2011/07/30/rendering-to-graphics-in-aspose.words-for-java-10.3/
author: Romank
summary: ''
tags: ['BMP', 'JPEG', 'PNG', 'Word', 'java', 'product release']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-java.png" alt="">}}


We have just released the first iteration of the "render to graphics" feature in [Aspose.Words for Java 10.3][1]. Rendering to graphics has been available in Aspose.Words for .NET for long time, but we managed to port it to Java only now. This functionality shines through in several important places in Aspose.Words. The following is a summary of what is now available.

## Render Word Document Pages to PNG, BMP and JPEG

It is now possible to convert any Microsoft Word document pages into a raster image. Just use the Document.Save method, specify the options using the ImageSaveOptions and specify the save format using one of the new SaveFormat enumeration values: PNG, BMP or JPEG.

This can be used for creating page thumbnails of various sizes.

## Render Shapes to HTML-based Formats

Aspose.Words for Java now faithfully renders all Microsoft Word drawing objects into raster images:

*   AutoShapes (pre-Word 2007 as well as the newer DrawingML shapes)
*   Textboxes
*   Images, including EMF and WMF metafiles
*   OLE objects

This ensures great results when converting documents to HTML-based formats (HTML, MHTML and EPUB).

## What's Next

We still have some "render to graphics" functionality that is available in Aspose.Words for .NET, but not in Aspose.Words for Java.

Here is the list of what you are going to see appearing in Aspose.Words for Java over the next few releases:

*   Saving document pages to multi frame TIFF.
*   Settings such as resolution, pixel format, image color mode in the public API.
*   Document.RenderToScale and Document.RenderToSize methods to render page directly onto a Java's Graphics2D object.
*   Rendering of individual shapes from the document.
*   Printing of documents.




[1]: https://downloads.aspose.com/words/java




