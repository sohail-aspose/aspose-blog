---
title: 'Work with Document Properties and Support of Notes Slide in Aspose.Slides for .NET 15.6.0'
date: Wed, 29 Jul 2015 19:16:36 +0000
draft: false
url: /2015/07/29/improved-api-to-work-with-document-properties-and-notes-slides-management-in-presentations/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-net_100.png" alt="">}}


We are pleased to share the release announcement for [Aspose.Slides for .NET][1] 15.6.0. This is one of the maintenance releases whereby we have added some new features as well.

## New Features

We have improved the support for working with document properties by introducing the feature for cleaning added document properties. Please visit the documentation article [Public API and Backwards Incompatible Changes in Aspose.Slides for .NET 15.6.0][2] for further reference. We have improved the management of notes slides by introducing NotesSlideManger class under ISlide interface. Now you can add or remove the notes slides for any given slide by using properties available in NotesSlideManager class. We have also introduced the support for exception messages when loading the files other than support MS PowerPoint formats.

## Resolved Issues

We have improved the support for presentations access and their saving that resulted in the generation of corrupted presentations and raising presentation repair messages when opened in PowerPoint. The presentation access and saving issues have been rectified for many presentation decks that earlier resulted in exceptions including NullReference, ArgumentException, OdpReadException, PptException, Unexpected Font Parsing and PptUnsupportedFormatException in previous releases during saving and exporting to Pdf.

We have improved the charting support in this new release and many issues incurring during working with charts have been rectified which include issues with chart labels, axis, plot area, data formats, and chart legends. Slide cloning has also been improved which earlier resulted in missing data in the form of improper shapes, tables, and charts inside cloned slides.

The support for working with SmartArt shapes has been improved and now hyperlinks or effects can be associated with SmartArt shapes. We have also included the text AutoFit and Wrapping support for the chart data item.

We have enhanced the presentation rendering to HTML, PDF, and images in this release for charts, text, and SmartArt shapes. Many chart rendering issues including missing or improper chart axis, plot area, and legends have been rectified. The issues of missing charts including the issue of improper chart leader lines have also been rectified in this release. We have also addressed the rendering issues related to AutoShapes and Smart as well in this release.

We have made several enhancements to the new API. Refer to the article [Public API and Backwards Incompatible Changes in Aspose.Slides for .NET 15.6.0][3] for further reference.

To see a complete list of fixes and to download Aspose.Slides for .NET 15.6.0, [please visit the download page][4].




[1]: https://products.aspose.com/slides/net
[2]: https://docs.aspose.com/display/slidesnet/Public+API+and+Backwards+Incompatible+Changes+in+Aspose.Slides+for+.NET+15.6.0
[3]: https://docs.aspose.com/display/slidesnet/Public+API+and+Backwards+Incompatible+Changes+in+Aspose.Slides+for+.NET+15.6.0
[4]: https://downloads.aspose.com/slides/net




