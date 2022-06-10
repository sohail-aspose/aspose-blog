---
title: 'Feature Rich OMR Template Editor with Aspose.OCR for .NET 2.7.0'
date: Wed, 01 Jul 2015 18:05:01 +0000
draft: false
url: /2015/07/01/introducing-feature-rich-omr-template-editor-with-aspose.ocr-for-.net-2.7.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce that [Aspose.OCR for .NET][1] 2.7.0 is now available for public use. This release has improved the **OMR Template Editor** by adding more features including the Aspose.BarCode support in Java mode, support for different types of Symbologies for the BarcodeElement, and setting the Threshold Level. Please review the release notes of Aspose.OCR for .NET 2.7.0 for a complete list of new features & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you check the Public API Changes section to know what has been changed since your current revision of the API.

While you're downloading the latest version, here is a glance at the most worth mentioning features of this release.

## New Features

There are some new features introduced in this release.

*   OMR Template Editor now provides support to configure [Aspose.BarCode for Java][2] when Template Editor is working Java mode. You can supply the Aspose.BarCode Jar file to the editor by switching first switching it to Java mode on the General tab and then accessing the Aspose.BarCode Setup tab.
*   OMR Template Editor now provides a Type property associated with BarcodeElement. Using Type property you will be able to manage the symbologies of the Barcode used in the template.
*   The threshold value shows how many pixels of the mark must be black in order to consider the mark as filled. Now OMR Template Editor provides an interface that helps to manage the threshold values used while performing OMR operation.
*   Aspose.OCR for .NET provides facility to perform OCR operation on remote images as well as local ones. You just need to supply the URL of the image to the newly exposed _**FromUrl**_ method. Following is the simple code snippet demonstrating the usage of the said method to perform OCR on a remote image.

```
OcrEngine ocrEngine = new OcrEngine();
ocrEngine.Image = ImageStream.FromUrl("http://www.someplace.com/images/logo.gif"); 
```

## Enhancements

This release has incorporated some enhancements. The list of enhancements is given below.

*   Copy and Paste multiple selected items support for OMR elements on the template using hotkeys as well as mouse shortcut menu.
*   Improved OcrEngine to handle distorted and low-resolution images.
*   Improved OmrEngine to handle marks filled with a pencil.

## Aspose.OCR for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for .NET API][3].
*   [Download Aspose.OCR for .NET][4].
*   [Aspose.OCR for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://products.aspose.com/ocr
[2]: https://products.aspose.com/barcode/java
[3]: https://products.aspose.com/ocr/net
[4]: https://downloads.aspose.com/ocr/net
[5]: https://docs.aspose.com/display/ocrnet/Home
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[9]: http://forum.aspose.com




