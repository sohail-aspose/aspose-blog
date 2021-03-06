---
title: 'Crop Image in Word to PDF and XPS using C# or VB.NET'
date: Thu, 06 Aug 2009 16:11:00 +0000
draft: false
url: /2009/08/06/aspose-words-now-supports-image-cropping-is-output-to-pdf-xps-printing-and-images/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have just released [Aspose.Words for .NET 6.6][1] that (among other great things) includes a new feature that I really wanted to mention.

Support for proper **rendering of cropped images** has been missing for long time and requested by too many customers. An image in a Microsoft Word document can be cropped and Aspose.Words used to ignore the crop settings when rendering to PDF, XPS, Graphics or printing. I am happy to announce that rendering of cropped images is now fully supported. The following are some screenshots to demonstrate.

## Original Document in Microsoft Word

Here is the test document opened in Microsoft Word.

## Aspose.Words rendered to PDF and XPS

The images below show how the above document was converted by Aspose.Words to PDF and XPS.

I would like to draw you attention to the following details:

*   Some images are raster and some are metafiles. Aspose.Words correctly crops both.
*   Both inward and outward cropping is supported.
*   When the image is cropped outward, then the shape background becomes visible.
*   The shape background can be a fill color, gradient, texture or pattern. Color, texture and pattern are supported. Gradients are not yet completely supported in all output formats.
*   Rotation and images in groups are included in the test and supported.

## Metafiles are Rendered as Vector Graphics

Although this feature has been available in rendering since the beginning, I feel it is worthwhile to mention.

WMF and EMF metafiles are vector images and these formats cannot be natively embedded in PDF or XPS documents. Aspose.Words goes to great lengths to parse metafiles and faitfully convert them to appropriate vector graphics so your output documents stay small in size and display beatifully at any zoom level or during printing. It is not a trivial job to convert metafiles to vector graphics and also crop them, so this is just one of the many features that we are proud of.

The following pictures show the same PDF and XPS documents generated by Aspose.Words but at high zoom.




[1]: https://downloads.aspose.com/words/net




