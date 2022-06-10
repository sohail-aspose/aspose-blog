---
title: 'Merged OCR &amp; OMR Features with Aspose.OCR for .NET 2.4.0'
date: Wed, 01 Apr 2015 17:53:06 +0000
draft: false
url: /2015/04/01/merged-ocr-omr-features-with-aspose.ocr-for-.net-2.4.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---

![Aspose.OCR for .NET logo][1]We're pleased to announce the release of the first version of merged Aspose.OCR for .NET. In this merged version, we have combined the Aspose.OCR & Aspose.OMR namespaces in one assembly and published it as [Aspose.OCR for .NET 2.4.0][2]. Now you can use the single component to work with both OCR & OMR features without even changing your existing code. If you are planning to upgrade the API from any revision prior to v2.3.0, we would strongly suggest you to check the Public API Changes section first.

## What Has Been Changed?

From API point of view, nothing has changed. All the classes, method, enumerations & properties that were previously present in Aspose.OMR namespace still reside there, whereas all the APIs relevant to OCR features still belong to Aspose.OCR namespace.  In order to keep this transition simple, we haven't changed anything in the public API so you do not need to worry about changing your existing code to accommodate this merger. However, number of assemblies for the Aspose.OCR for .NET package have been reduced to one, that mean; you can use the single assembly (Aspose.OCR.dll) for both OCR & OMR features from now onward. Please review the Public API Changes in reference to Aspose.OCR for .NET 2.4.0 for more details.

## Enhancements & Fixes

This release has addressed a few critical issues and has incorporated some enhancements as detailed below.

*   Fixed the implementation of IRecognitionBlock.RecognitionData that used to return null for the custom recognition blocks. Due to this issue, the API didn't allow to retrieve the symbols & words that belongs to a specific block on image.
*   Fixed the problem with invalid overloaded comparer that used to trigger the ArgumentException at OcrEngine.Process.
*   Improved the exception handling for the cases where OMR elements have invalid dimensions.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-net_100.png "Aspose.OCR for .NET"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/entry618205.aspx "Download Aspose.OCR for .NET 2.4.0"
[3]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx




