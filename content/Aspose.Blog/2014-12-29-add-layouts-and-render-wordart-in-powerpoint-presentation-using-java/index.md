---
title: 'Add Layouts and Render WordArt in PowerPoint Presentation using Java'
date: Mon, 29 Dec 2014 17:43:29 +0000
draft: false
url: /2014/12/29/add-layouts-and-render-wordart-in-powerpoint-presentation-using-java/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-Java_100.png" alt="">}}


We're pleased to announce the release of [Aspose.Slides for Java][1] 14.10.0. This is a major product release where we have included support for WordArt and some new features. We have also address many rendering as well as presentation access and export issues that have been reported for exported PDF, HTML and slide thumbnails in earlier versions.

## New Features

We have introduced the support for generating the HTML file for independent presentation slides as well in this release. Now, one can generate the HTML file per slide by following the documentation link, Converting individual Slide to HTML in a Presentation. We have also introduced the support for WordArt rendering in this new API. Now, the generated slide thumbnails, exported PDF, Tiff and SVG will render WordArt shapes properly if they are added in presentation slides. The support for adding the layout slides in a presentation if the desired layout type is missing in layout slides collection of used master slide has also been made available in this release. More details about this feature are available in the article Adding Layout Slides to Presentation.

We have also included the support for generating the slide thumbnail for user defined portion of the slide in this release that has been requested by some of customers. For further details about the feature support please visit the documentation article Generating a Thumbnail of User Defined Window from a Slide. The support for extracting the audio data from slide transition effects has also been included. For more information about the this feature, please visit the article Extracting Audio Used In SlideShow Transitions.

## Resolved Issues

We have rectified several incurring issues with API in this release which include the issues pertaining to loading license of Aspose.Slides for Java. The issue of Aspose.Slides failing to work when used in background thread has also been resolved. The API earlier had issue with added videos and it failed to load the videos in PowerPoint slides. The said issue has been addressed along with issue of chart failing to get opened in PowerPoint as well.

We have improved the presentation rendering support and have resolved certain rendering issues incurring during generation of slide thumbnails, exported PDF, Tiff, SVG and XPS files. The issues include improper text, missing background, blank slides, missing WordArt, improper SmartArt and different charts elements rendering.

We have rectified issues that appeared when accessing, saving and rendering presentation to PDF, HTML or slide thumbnails, which resulted in different exceptions like NullReference, KeyNotFoundException, PptxReadException, ObjectReferenceException,and IndexOutOfRange in previous releases for MAC, Windows and Java environments.

We have made several enhancements to the new API. Refer to the article Public API and Backwards Incompatible Changes in Aspose.Slides for Java 14.10.0 for further reference.

To see a complete list of fixes and to download Aspose.Slides for Java 14.10.0, [please visit the download page][2].




[1]: https://products.aspose.com/slides/java
[2]: https://downloads.aspose.com/slides/java




