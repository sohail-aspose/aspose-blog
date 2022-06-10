---
title: 'Supply multiple whitelists for single OCR operation with Aspose.OCR for .Net 16.10'
date: Thu, 13 Oct 2016 05:59:52 +0000
draft: false
url: /2016/10/13/supply-multiple-whitelists-for-single-ocr-operation-with-aspose.ocr-for-.net-16.10/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-net_100.png) We are pleased to announce the release of Aspose.OCR for .Net 16.10. The major development in this release is support for supplying multiple white lists for single OCR operation. Improved process of barcode recognition from OMR sheet has also been incorporated in this release.

## Supply Multiple White Lists

Aspose.OCR for .Net provides the functionality to perform the OCR operation with more than one white list for a single OCR operation. Aspose.OCR for .Net API has introduced a new property Whitelist in RecognitionBlock class. With the help of this property developer can set white list for each RecognitionBlock introduced in a single OCR process. Below provided code snippet demonstrates how to process multiple RecognitionBlock with their own white list in a single OCR operation.

```
 // Create an initialize an instance of OcrEngine
OcrEngine engine = new OcrEngine();

// Set the OcrEngine.Image property by loading an image from disk, memory or URL
engine.Image = ImageStream.FromFile("sample.jpg");


// create text recognition block by supplying X,Y coordinates and Width,Height values
IRecognitionBlock block = RecognitionBlock.CreateTextBlock(6, 9, 120, 129);

// set the Whitelist property by specifying a new block whitelist
block.Whitelist = new char[] { '0', '1', '2', '3', '4', '5', '6', '7', '8', '9' };

// YOU CAN ADD MORE TEXT BLOCK AND SET WHITE LISTS.

// set different configurations and add recognition block(s)
ocr.Config.ClearRecognitionBlocks();
ocr.Config.AddRecognitionBlock(block);
ocr.Config.DetectTextRegions = false;

// Call OcrEngine.Process method to perform OCR operation
if (engine.Process())
{
    // Display the recognized text from each Page
    Console.WriteLine(engine.Text);
} 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of loading barcode into the OMR template editor has been improved.
*   Working of barcode recognition into the OMR template editor has been improved.

Please check the release notes of [Aspose.OCR for .Net 16.10][2] for a complete list of enhancements.

## Aspose.OCR for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for .Net API][3].
*   [Download Aspose.OCR for .NET][4].
*   [Aspose.OCR for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-net_100.png "Aspose.OCR for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/default.aspx
[3]: https://www.aspose.com/products/ocr/net
[4]: https://downloads.aspose.com/ocr/net
[5]: https://docs.aspose.com/display/ocrnet/Home
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[9]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx




