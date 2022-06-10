---
title: 'Autoporting Aspose.Words for Java Progress - 24th Nov 2010'
date: Wed, 24 Nov 2010 12:25:00 +0000
draft: false
url: /2010/11/24/autoporting-aspose-words-for-java-progress-24th-nov-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Today we have a completely autoported Aspose.Words for Java compile for the first time!

There are 2470 source files in the project. Only 28 of them constitute the platform abstraction layer and are manually coded in Java. The rest of the Java sources are generated from our C# sources.

Now the race is on to get all Aspose.Words for Java unit tests to pass. I will continue to provide regular updates about progress.

As a heads up for you, here is a preliminary list of features that will not be (yet) available in Aspose.Words for Java. The items on this list are singnificantly less severe limitations than we had before in Aspose.Words for Java. Everything else that you don't see here (including support for WordML 2003, EPUB, PDF, XPS, SWF, field update, TOC, nested mail merge regions etc) is supported!

  

**Limitation**

**Severity**

**Comment**

No rendering to images or printing (GDI Renderer).

Medium

More platform dependent work needed in graphics. No big problems, just leave till next version.

All Renderers/Gdi classes made msonly.

Brightness, contrast, grayscale/bw transform not supported when rendering shapes with images.

Minor

ImageColorFilter.cs made msonly.

It should be possible to do using just the standard Java libraries, just need a bit more time.

CCITT3 and CCITT4 (TIFF) compression not supported in rendering to PDF.

Minor

When saving images using CCITT compression in .NET we use the GDI+ codec to write the TIFF data.

It should be possible in Java too if JAI is installed and TIFF codec is available, but just needs a bit more time.

ImageEncoder.cs made msonly.

BitonalConverter.cs made msonly.

TiffData.cs made msonly.

Image cropping is not supported.

Medium

This should be possible in Java. Just needs a bit more time.

2010-11-21 RK I actually have some cropping code on Java in PalBitmap. So some cropping is supported, need to look at this.

WordArt text is not rendered.

Medium

We use GDI+ feature that converts text into graphics paths. Graphics path is a GDI+ object. We need to have the capability to convert text to graphics path and to represent graphics path in Java to do that.

2010-11-20 Came up with the idea of "simplified WordArt rendering" using ApsGlyphs instead of ApsPath. Asked DB to implement this as an option in C#. Then I will be able to autoport it to Java.

Metafile rendering to vector graphics does not fallback to raster.

Known Issue

In our .NET code, when we are rendering EMF or WMF into PDF or XPS - we render it as vector graphics (APS). But if during rendering we encounter a record that we do not support and know it will cause loss of visual fidelity (for example PatInvent) - we fallback onto using GDI+ to render metafile as a raster image. We then output the raster image into PDF or XPS. Obviously in Java we do not have any fallback alternative and the output will just have to appear incorrect.

ChromaKey on image (Opacity mask by color) is not supported when rendering to XPS

Medium

This requires bitmap pixel manipulation. Do later in Java.

Rescaling image, converting metafile to raster and cropping is excluded from HTML exports.

2010-11-23 This is temporary just to get code autoported asap. We can turn rescaling and cropping back on, but no metafile to raster conversion yet.

Digitally signing PDF documents.

Uses .NET X509Certificate2, need a bit of work to make platform independent.

Verification of digital signatures DOC, DOCX and ODT

Uses .NET cryptography, needs a bit work to make platform independent.

Find and Replace with regular expression can use group indexes, but cannot use group names.

Minor

Java regex does not support group names, it supports only group indexes. This is rarely used advanced feature. Using indexes is still possible, so no user impact.








