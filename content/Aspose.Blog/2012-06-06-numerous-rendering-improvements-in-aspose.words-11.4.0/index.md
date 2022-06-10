---
title: 'Numerous Rendering Improvements in Aspose.Words 11.4.0'
date: Wed, 06 Jun 2012 15:46:21 +0000
draft: false
url: /2012/06/06/numerous-rendering-improvements-in-aspose.words-11.4.0/
author: Adam Skelton
summary: ''
tags: ['DeviceGray', 'DeviceRGB', 'EMF', 'Enhanced MetaFile', 'Enhanced Metafile Plus', 'OfficeMath', 'Printing', 'rendering']
categories: ['Aspose.Words Product Family']
---

![](http://www.aspose.com/Images/aspose.words-logo2.jpg "Aspose Logo")During the month we have been hard at work and it shows, as this month's release contains 112 improvements and fixes.

You can download it straight away from:

*   [Aspose.Words for .NET 11.4.0][1]
*   [Aspose.Words for Java 11.4.0][2]

Both of these releases contain many new features and bug fixes across all of the different areas of Aspose.Words. In the rest of this post, I will focus on looking at a couple of the cool new rendering features on offer:

## Improved Rendering of Black Colors to PDF for Proper Printing

Aspose.Words strives to export documents just like they appear in Microsoft Word. We are also in-tune with our customers and listen to their requests and implement any changes where helps.

### The Problem

We were alerted to an issue by one of our customers that Aspose.Words renders black or gray color to PDF not as **“true black”** but only as **“rich black”.** The difference between these two colors is only a PDF with “true black” content is actually printed using pure black ink only. On the other hand content that is **“rich black”** is printed using a combination of colored and black ink. In a professional printing house, having a document which is printed incorrectly or uses more ink than required is unacceptable. We promised to fix this issue in Aspose.Words:

### Aspose’s Solution

Since Microsoft Word exports PDF documents with correct behavior we knew this was a bug which required a fix as soon as possible. Our developer responsible for this area worked hard and a few weeks after the customer originally reported the issue the bug was resolved. The fix for this issue is included in this month’s release of both Aspose.Words for .NET and Aspose.Words for Java.

### The Result

Aspose.Words now exports gray and black color to PDF the same way as how Microsoft Word does. Such color is now exported in the **DeviceGray** color space and all other types of colors are exported in **DeviceRGB**. This exports colors correctly as **“true black”** as the customer originally wanted.

## Support for Rendering of EMF+ Metafiles

### What is EMF and EMF+?

**Enhanced** **Windows Metafile** (**EMF**) is a graphics file format on Microsoft Windows systems which are intended to be portable between applications and may contain both vector graphics and bitmap components. It acts in a similar manner to SVG files.

**Enhanced Windows Metafile Plus (EMF+)** technology builds on EMF and allows the vector image to have access to advanced features such as anti-aliased 2D graphics, floating point coordinates, gradient shading and more.

### Support for EMF and EMF+ in Aspose.Words

Aspose.Words already boasts support for rendering embedded EMF images to other formats such as PDF and image. Now rendering EMF+ metafiles can be added to the list of supported features as well.

There have been several customers whose documents contain EMF+ metafiles. In previous versions of Aspose.Words the rendered version of their documents may have looked incomplete due to missing support for EMF+. This technology is actually complex and it took a lot of effort to implement it. We are proud to announce that EMF+ content is now supported during rendering by Aspose.Words.

## Further Improvements to OfficeMath Rendering

In our previous month’s post we blogged about how our new support for rendering OfficeMath objects to formats such as PDF and image. The post detailed a few sub features that were not supported.

We have continued work on this feature and have already implemented some of the missing functionality. Here is a list of improvements to OfficeMath rendering in this release:

*   All variants of fraction are now supported.
*   Support for vertical alignment of elements in equations.
*   Fixed a bug where glyphs in Cambria Math were rendered higher than needed. This bug prevented OfficeMath from being properly rendered to vector based formats.
*   Support for column and row spacing in matrix and array.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




