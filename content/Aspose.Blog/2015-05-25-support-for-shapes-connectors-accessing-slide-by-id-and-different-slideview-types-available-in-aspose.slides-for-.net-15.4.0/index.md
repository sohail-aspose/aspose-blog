---
title: 'Different SlideView Types for PowerPoint Presentations - .NET PowerPoint API'
date: Mon, 25 May 2015 07:36:12 +0000
draft: false
url: /2015/05/25/support-for-shapes-connectors-accessing-slide-by-id-and-different-slideview-types-available-in-aspose.slides-for-.net-15.4.0/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-net_100.png" alt="">}}


We like to share the release announcement for [Aspose.Slides for .NET][1] 15.4.0. This is one of the maintenance releases in which we have resolved certain issues incurring in the product along with some of new features.

## New Features

We have included the long-awaited support for joining the shapes using connectors. Please visit the documentation article, [Connecting shapes using Connectors][2] for more details and sample code. We have also resumed the support for getting slide by ID using GetSlideById(id) method exposed by the Presentation class. We have also included the support for setting the predefined view type for the generated presentation when it gets opened in PowerPoint. The slide view type can be set using ViewProperties exposed by the Presentation class.

We have also improved the Table support in Aspose.Slides and have added the facility for splitting the table cells based row span, column-span, split by height and split by width. We have also added the support for working with NotesSlides and one can now use MasterNotesSlideManager exposed by Presentation class to access the NotesMaster and its elements.

## Resolved Issues

We have resolved the issues that appeared while accessing, saving, and rendering presentation to PDF, HTML or slide thumbnails, which resulted in different exceptions like NullReference, ArgumentException , UnSupportedBrushTypeException, and IndexOutOfRange in previous releases. The issue of presentation repair message appearing in Aspose.Slides generated presentations when viewed in different PowerPoint versions has also been addressed and resolved in this release. A step forward has also been taken towards improving the performance of API in terms of memory usage as well.

We have addressed many text and image rendering issues in this new release that occurred in charts, tables, Smart, and AutoShape. We have also improved the strike-through text rendering support for generated PDF and thumbnails. Many of chart elements rendering issues including chart titles, axis text, legends, and chart labels have been addressed for different type of charts. The rendering performance has been significantly improved for generated thumbnails, exported Pdf, and SVG files. The WordArt rendering has also been improved in this new release and the issue of WordArt effects getting lost in exported output has been rectified. The issue related to corrupt PDF files generated while exporting presentations with WordArt to PDF has also been addressed.

We have made several enhancements to the new API. Refer to the article Public API and Backwards Incompatible Changes in Aspose.Slides for .NET 15.4.0 for further reference.

To see a complete list of fixes and to download Aspose.Slides for .NET 15.4.0, [please visit the download page][3].




[1]: https://products.aspose.com/slides/net
[2]: https://docs.aspose.com/display/slidesnet/Shape+Manipulations#ShapeManipulations-Connectingshapesusingconnectors
[3]: https://downloads.aspose.com/slides/net




