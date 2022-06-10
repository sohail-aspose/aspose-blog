---
title: 'WordArt 3D Lighting Rendering, Many DrawingML Improvements and New Reporting Engine in Aspose.Words 14.9.0'
date: Tue, 21 Oct 2014 12:14:11 +0000
draft: false
url: /2014/10/21/wordart-3d-lighting-rendering-many-drawingml-improvements-and-new-reporting-engine-in-aspose.words-14.9.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 14.9.0 has been released. This month’s release contains over 120 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.9.0][1]
*   [Aspose.Words for Java 14.9.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   New reporting engine allows developers to use LINQ method syntax in report templates.
*   Support for databinding for image SDTs.
*   DrawingML is now a composite node (breaking change to the public API).
*   DrawingML supports linked textboxes.
*   Improved rendering of 'keep with next' paragraphs.
*   Implemented 'use printer metrics to lay out document' compatibility option (Windows/GDI only).
*   Improved tabs handling logic for Word 2013 and compatible modes in rendering.
*   Extrusion effect for DrawingML shapes rendering implemented (cold rendering).
*   Rounding corners rendering in DrawingML charts implemented.
*   Improved 3D lighting rendering for WordArt objects.
*   Added support of Gradient background in HTML output.

## DrawingML is Now a CompositeNode

The DrawingML node is now CompositeNode. That is why the VisitDrawingML method in DocumentVisitor was replaced with VisitDrawingMLStart and VisitDrawingMLEnd.

## Extrusion Effect for DrawingML Supported

We have added support for the extrusion effect to DrawingML. To enable this effect, set the flag SaveOptions.DmlRenderingMode to DmlRenderingMode.DrawingML. By defaultm SaveOptions.DmlRenderingMode is set to DmlRenderingMode.Fallback.

## LayoutEnumerator Supports Moving between Logical Siblings

We have added two new members to LayoutEnumerator. It is now possible to move between logical siblings and thus find, for example, where a paragraph is broken across pages.

```
 // LayoutEnumerator.MoveNextLogical Method
public bool MoveNextLogical();

// LayoutEnumerator.MovePreviousLogical Method
public bool MovePreviousLogical(); 
```

## Mail Merge Classes Moved to the Aspose.Words.MailMerging Namespace

We decided to move mail merge classes from the Aspose.Words.Reporting namespace to Aspose.Words.MailMerging. Our customers should not confuse these classes with the new reporting engine's classes that belong to the Aspose.Words.Reporting namespace. For this reason our customers need to change the 'using' directives in their source code accordingly to be able to use new versions of Aspose.Words. This is an intentional breaking change.

This is a breaking change in Aspose.Words for .NET only. In Aspose.Words for Java, all classes are in the com.aspose.words package and therefore there is no breaking change.

## New Reporting Engine

This release includes the new reporting engine that supports LINQ method syntax in report templates. The classes of the reporting engine are located in the Aspose.Words.Reporting namespace. Note that the new reporting engine is not yet available in Aspose.Words for Java. It will be hopefully available in the next release.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




