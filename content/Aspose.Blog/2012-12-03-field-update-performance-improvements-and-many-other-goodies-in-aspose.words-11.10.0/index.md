---
title: 'Field Update Performance Improvements, and Many Other Goodies in Aspose.Words 11.10.0'
date: Mon, 03 Dec 2012 12:01:37 +0000
draft: false
url: /2012/12/03/field-update-performance-improvements-and-many-other-goodies-in-aspose.words-11.10.0/
author: Adam Skelton
summary: ''
tags: ['JPEG image compression', 'OOXML charts', 'TOC', 'Table of contents', 'field update', 'performance']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_.png" alt="">}}


We are happy to announce this month’s release of improvements to Aspose.Words for .NET and Java. This release contains 157 improvements to Aspose.Words, including several great performance and space-saving benefits.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.10.0][1]
*   [Aspose.Words for Java 11.10.0][2]

## Dramatic Improvement to Table of Contents Field Update Performance

In this release, we have tweaked the impressive algorithm Aspose.Words uses to regenerate table of contents (TOC field) just like how Microsoft Word displays it.  After upgrading to this release you can expect up to 50% increase in field update speed when updating documents that contain a TOC field, this includes when updating fields (calling **Document.UpdateFields** through the API) or rendering a document (saving to PDF, XPS, image and so forth).

Under the hood, this fix greatly improves the speed PAGEREF fields are updated therefore there may be other documents which don’t contain a table of contents that also gain a boost performance during field update.

## Choose Image Compression when saving to PDF

This month’s release introduces a new save option member to specify the image compression when saving to PDF. Normally images are rendered in the format they appear in the input document, this can often mean a lossless compression format called Flate compression is used which provides great quality but can cause an increase in file size.

You can now use **PdfSaveOptions.ImageCompression** to specify JPEG compression. Use this option in conjunction with the existing **PdfSaveOptions.JpegCompression** option to fully control the level of compression and space saving benefits.

```
Document doc = new Document("Document.doc");

PdfSaveOptions options = new PdfSaveOptions();

// Using JPEG compression at 50% quality
options.ImageCompression = PdfImageCompression.Jpeg;
options.JpegQuality = 50;

doc.Save("Document Out.pdf", options);
```

## Improvements to OOXML Chart Rendering

This release furthers the work we are doing to fully support OOXML chart rendering. These charts are found in the newer versions of Microsoft Word documents.

In addition to the features Aspose.Words already supports when rendering OOXML charts, this month's improvements also adds the following features to the list:

*   Legend
*   Chart Title
*   Axis Title (partially supported)
*   Data Labels (partiaully supported)
*   Error Bars
*   Picture Shapes and Textboxes
*   Axis
*   Data Point
*   Legend
*   Font
*   Manual Layout
*   Overlapping




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




