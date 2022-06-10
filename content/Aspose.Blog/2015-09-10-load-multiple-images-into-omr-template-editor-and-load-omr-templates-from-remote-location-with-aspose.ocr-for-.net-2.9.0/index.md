---
title: 'Load Multiple Images into OMR Template Editor in C#'
date: Thu, 10 Sep 2015 06:53:43 +0000
draft: false
url: /2015/09/10/load-multiple-images-into-omr-template-editor-and-load-omr-templates-from-remote-location-with-aspose.ocr-for-.net-2.9.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We like to announce the release of Aspose.OCR for .NET 2.9.0. This release includes a new OmrImage property to load the template from a remote location. Please review the release notes of [Aspose.OCR for .NET 2.9.0][1] for a complete list of new feature & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you check the Public API Changes section to know what has been changed since your current revision of the API.

## Load Multiple Images into OMR Template Editor

OMR Template Editor now provides support to load multiple scanned images into template editor and perform OMR operation simultaneously.

Run the OMR Template Editor tool. Go to the Page menu, select Import Multiple Images. An open dialog appears to offer you to select images in PNG, JPG, GIF, TIF or BMP format.



{{< figure align=center src="images/omr_editor-300x112.jpg" alt="">}}


Note that Page toolbar has been enabled and shows the total number of images loaded. Now you can move between image sheets using left (<) & right (>) arrows on the Page toolbar.

In order to extract the data from scanned images, simply click the _Extract Data_ button on the toolbar. The _Data Extraction Results_ window will appear. The window contains different tabs. Each tab shows the output/result from a respective image sheet.



{{< figure align=center src="images/multipage_result-300x168.jpg" alt="">}}


## Load OMR Template from URL

Aspose.OCR for .NET provides facility to load OMR template from a remote location as well as the images available on local disk. You just need to supply the URL of the OMR template to newly exposed LoadFromUrl method.

Following is the simple code snippet demonstrating the usage of the said method to load OMR template from a remote location.

```
string templateUrl = "https://sampleurl.com/sample.amr";

// Initialize an instance of OmrTemplate by loading the OMR template from URL
OmrTemplate template = OmrTemplate.LoadFromUrl(templateUrl);

//Do Processing

```

## Aspose.OCR for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for .NET API][2].
*   [Download Aspose.OCR for .NET][3].
*   [Aspose.OCR for .NET online documentation][4] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][8] for a chat.




[1]: https://downloads.aspose.com/ocr/net
[2]: https://products.aspose.com/ocr/net
[3]: https://downloads.aspose.com/ocr/net
[4]: https://docs.aspose.com/display/ocrnet/Home
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[7]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[8]: http://forum.aspose.com




