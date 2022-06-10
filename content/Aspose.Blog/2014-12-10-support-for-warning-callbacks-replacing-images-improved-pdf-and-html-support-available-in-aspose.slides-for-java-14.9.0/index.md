---
title: 'Support for Warning Callbacks, Replacing Images, Improved PDF and HTML Support in Aspose.Slides for Java 14.9.0'
date: Wed, 10 Dec 2014 09:51:17 +0000
draft: false
url: /2014/12/10/support-for-warning-callbacks-replacing-images-improved-pdf-and-html-support-available-in-aspose.slides-for-java-14.9.0/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-Java_100.png" alt="">}}


We're pleased to announce the release of Aspose.Slides for Java 14.9.0. This is a major product release where we have included support for some new features. We have also address many rendering as well as presentation access and export issues that have been reported for exported PDF, HTML and slide thumbnails in earlier versions.

## New Features

We have introduced support for replacing an image in a presentation image collection with a different one. As a result of this, the image is replaced in all instances in the presentation that refers to it. Please read the article [Replacing Images in the Presentation Image Collection][1] for further details. We have also introduced support for setting the fill format for SmartArt nodes and you can now set the fill color or pattern for SmartArt nodes. More details about this feature are available in the article [Setting Fill Format for SmartArt Node][2].

We have introduced support for generating a PDF for a specific number of slides. You can find more details by visiting and reading the article [Exporting Presentation to PDF][3]. Support for generating HTML files for individual presentation slides has also been included in this new release. More details about this feature are available in the article [Converting Individual Slide to HTML][4].

Now, Aspose.Slides for Java makes it possible to get warning callbacks for font substitution in case the used font is not available on the machine during the rendering process. Warning callbacks are helpful when debugging issues of missing or inaccessible fonts during rendering. You can find more details about this feature by visiting the article [Getting Warning Callbacks for Fonts Substitution in Aspose.Slides][5].

## Resolved Issues

We have rectified exception issues that appeared when accessing, saving, and rendering presentation to PDF, HTML, or slide thumbnails, which resulted in different exceptions like KeyNotFoundException, UnKnownFileFormatException, NullReference, ArgumentException, and IndexOutOfRange in previous releases.

We have taken a leap towards improving the presentation rendering support for exported PDF, SVG, HTML, and slide thumbnails in this release. Several issues pertaining to improper text, wrong shape, improper charts, unfitting SmartArt, and wrong font rendering have been addressed in this regard.

We have made several enhancements to the new API. Refer to the article [Public API and Backwards Incompatible Changes in Aspose.Slides for Java 14.9.0][6] for further reference.

To see a complete list of fixes and to download Aspose.Slides for Java 14.9.0, [please visit the download page][7].




[1]: https://docs.aspose.com/display/slidesjava/Replacing+Images+inside+Presentation+Image+Collection
[2]: https://docs.aspose.com/display/slidesjava/Setting+Fill+Format+for+SmartArt+Node+using+Aspose.Slides
[3]: https://docs.aspose.com/display/slidesjava/Converting+Presentation+to+PDF#ConvertingPresentationtoPDF-specificslides
[4]: https://docs.aspose.com/display/slidesjava/Converting+a+Presentation#ConvertingaPresentation-ConvertingPresentationtoHTML
[5]: https://docs.aspose.com/display/slidesjava/Getting+Warning+Callbacks+for+Fonts+Substitution+in+Aspose.Slides
[6]: https://docs.aspose.com/display/slidesjava/Public+API+and+Backwards+Incompatible+Changes+in+Aspose.Slides+for+Java+14.9.0
[7]: https://downloads.aspose.com/




