---
title: 'New Features for OMR Template Editor with Aspose.OCR for .NET 2.6.0'
date: Thu, 04 Jun 2015 09:10:05 +0000
draft: false
url: /2015/06/04/introducing-new-features-for-omr-template-editor-with-aspose.ocr-for-.net-2.6.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We’re pleased to announce the release of Aspose.OCR for .NET 2.6.0. The biggest attraction of this month’s release is the drag and drop OMR template into OMR Template Editor facility, directly copy paste OMR elements and support for GIF image instead of only JPG for scanned image of the template sheet. Please review the release notes of [Aspose.OCR for .NET 2.6.0][1] for a complete list of new features & enhancements. If you are planning to upgrade the API from any previous revision, go ahead there is no change in the API.

## New Features

There are some new features introduced in this release. Namely:

*   Drag And Drop support for OMR template (.amr) into OMR Template Editor.
*   Copy and Paste support for OMR elements on the template (using hot keys i.e. Ctrl+C & Ctrl+V).
*   GIF image support for import scan image of template sheet.

## Enhancements

This release has incorporated some enhancements. The list of enhancements is given below.

*   Freely edit the value/properties of over lapping elements.
*   Change in OMR element's count property takes place only on focus lost or enter key press of the property text box.
*   A new option has been introduced in order to customize/reset the resolution (DPI) of scanned image of the template sheet.
*   Setting the image resolution using OmrImage class.
*   Now OMR Template Editor needs no restart/exit and reload after setting valid license.

## Fixes

This release has also addressed 3 significant issues.

*   Get correct location of the recognized word while performing OCR on a scanned image.
*   In case of Choise Box OMR element, OMR engine will return empty string if Multiple Selection is set to NO. If it is set to YES then OMR engine will return both values.
*   Now the OMR Template Editor ('Extract Data from current sheet' option) and extracting OMR data from a scanned image using OmrEngine class retuns identical results.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][2] for a chat.




[1]: https://downloads.aspose.com/ocr/net
[2]: http://forum.aspose.com




