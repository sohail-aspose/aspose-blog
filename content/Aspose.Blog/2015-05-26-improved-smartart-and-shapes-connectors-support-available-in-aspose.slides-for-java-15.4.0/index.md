---
title: 'Improved SmartArt and Shapes Connectors for PowerPoint Presentations in Java'
date: Tue, 26 May 2015 17:59:11 +0000
draft: false
url: /2015/05/26/improved-smartart-and-shapes-connectors-support-available-in-aspose.slides-for-java-15.4.0/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-Java_100.png" alt="">}}


We're pleased to announce the release of [Aspose.Slides for Java][1] 15.4.0. This is one of maintenance release in which we have resolved certain issues incurring in the product along with support for some new features.

## New Features

We have introduced the support for joining the shapes using connectors in this release and now one can join the shapes using connector by selecting automatic shortest path or defining the connection point on shapes. Please visit the documentation article, Connecting shapes using Connectors for more details and sample code. We have also added the support for getting slide by ID using getSlideById(id) method exposed by Presentation class. The more details about this new feature can be explored in documentation article, Accessing slide by ID.

The SmartArt support has also been improved and some new features have been added when dealing with SmartArt shapes. Please visit documentation article, Exploring SmartArt Properties for more details in this regard. We have also included the support for setting the predefined view type for the generated presentation when it gets opened in PowerPoint. The slide view type can be set using ViewProperties exposed by Presentation class.

We have also improved the Table support in Aspose.Slides and have added the facility for splitting the table cells based row span, column span, split by height and split by width. We have also added the support for working with NotesSlides and one can now use MasterNotesSlideManager exposed by Presentation class to access the NotesMaster and its elements.

## Resolved Issues

We have improved the presentation rendering support and have resolved certain rendering issues incurring during generation of slide thumbnails, exported PDF, HTML and SVG files in Windows, Linux\\Unix and MAC platforms. The issues include improper text, missing background, missing strike through, improper SmartArt, improper gradient effects, incorrect table and different charts elements rendering. The WordArt rendering has also been improved in this new release and issue of WordArt effects getting lost in exported output has been rectified. The issue related to corrupt PDF file generated while exporting presentation with WordArt to PDF has also been addressed.

We have rectified issues that appeared when accessing, saving and rendering presentation to PDF, HTML or slide thumbnails, which resulted in different exceptions like NullReference, PptxReadException, ObjectReferenceException,and IllegalArgumentException in previous releases for MAC, Linux and Windows environments. The output of IWarningCallbacks has also been improved and now it is represented in a much informative way as well.

We have made several enhancements to the new API. Refer to the article Public API and Backwards Incompatible Changes in Aspose.Slides for Java 15.4.0 for further reference.

To see a complete list of fixes and to download Aspose.Slides for Java 15.4.0, [please visit the download page][2].




[1]: https://products.aspose.com/slides/java
[2]: https://downloads.aspose.com/slides




