---
title: 'Save Shape and OfficeMath Nodes to SVG in Aspose.Words 16.3.0'
date: Thu, 14 Apr 2016 14:29:45 +0000
draft: false
url: /2016/04/14/save-shape-and-officemath-nodes-to-svg-in-aspose.words/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)[Aspose.Words][1] 16.3.0 has been released. This month’s release contains over 87 useful new features, enhancements, and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.3.0][2]
*   [Aspose.Words for Java 16.3.0][3]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Support of Saving Shape and OfficeMath Nodes to SVG
*   Added Feature to Get-Set Shape's Aspect Ratio
*   Support for RC4 encryption
*   Reworked Public API for PlainTextDocument Creation
*   Renamed GetOpaqueRectangleInPixels to GetOpaqueBoundsInPixels in NodeRendererBase
*   Improvement of Transparent Image Rendering to PDFA-1

## Support of Saving Shape and OfficeMath Nodes to SVG

We have introduced new feature in Aspose.Words 16.3.0 to save OfficeMath formulas to image separately from whole document. Now it is possible to pass SaveFormat.Svg into ImageSaveOptions, so OfficeMath and Shape nodes can be save to SVG.

```
Document doc = new Document(@"C:\Temp\in.docx");
OfficeMath math = (OfficeMath)doc.GetChild(NodeType.OfficeMath, 0, true);
math.GetMathRenderer().Save(@"C:\Temp\formula.png", 
new ImageSaveOptions(SaveFormat.Png)); 
```

## Added Feature to Get-Set Shape's Aspect Ratio

We have introduced Shape.AspectRatioLocked property in Aspose.Words 16.3.0. Plase none that it is possible to get/set AspectRatioLocked for child shapes (mimic MS Word behavior), but AspectRatioLocked has effect only for top level shapes.

```
Shape shape = (Shape)doc.GetChild(NodeType.Shape, 0, true);

// Get/set AspectRatioLocked.
shape.AspectRatioLocked = true; 
```

## Reworked Public API for PlainTextDocument Creation

We have made following breaking API changes in 16.3.0 version:

*   All public overloads of static Document.ExtractText methods removed
*   PlaintextDocument class renamed to PlainTextDocument
*   Added 4 public constructors to the PlainTextDocument class with signatures corresponding to the removed static Document.ExtractText methods

## Renamed GetOpaqueRectangleInPixels to GetOpaqueBoundsInPixels in NodeRendererBase

We renamed GetOpaqueRectangleInPixels to GetOpaqueBoundsInPixels for names consistency and introduced GetBoundsInPixels method for consistency with other properties.

## Improvement of Transparent Image Rendering to PDFA-1

PDF/A-1 specification prohibits transparency. In order to provide better output Aspose.Words blends transparent images with white background. Previously images were blended only with PdfImageCompression.Auto. With PdfImageCompression.Jpeg transparent images were rendered by simply stripping alpha channels. Now images are blended for both PdfImageCompression.Auto and PdfImageCompression.Jpeg.




[1]: https://products.aspose.com/words
[2]: https://downloads.aspose.com/words/net
[3]: https://downloads.aspose.com/words/java




