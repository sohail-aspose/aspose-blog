---
title: 'Supply multiple whitelists for single OCR operation with Aspose.OCR for Java 16.10'
date: Thu, 27 Oct 2016 06:05:19 +0000
draft: false
url: /2016/10/27/supply-multiple-whitelists-for-single-ocr-operation-with-aspose.ocr-for-java-16.10/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png) We are pleased to announce that Aspose.OCR for Java 16.10 is now available for public use. The major development in this release is support for supplying multiple white lists for single OCR operation.

## Supply Multiple White Lists

Aspose.OCR for Java provides the functionality to perform the OCR operation with more than one white list for a single OCR operation. Aspose.OCR for Java API has introduced a new property setWhitelist in RecognitionBlock class. With the help of this property developer can set white list for each RecognitionBlock introduced in a single OCR process. Below provided code snippet demonstrates how to process multiple RecognitionBlock with their own white list in a single OCR operation.

```
 // Input file.
String sInputFile = "sample.jpg";

// Create an initialize an instance of OcrEngine
com.aspose.ocr.OcrEngine engine = new com.aspose.ocr.OcrEngine();

// Set the OcrEngine.Image property by loading an image from disk, memory or URL
engine.setImage(com.aspose.ocr.ImageStream.fromFile(sInputFile));

// Create text recognition block by supplying X,Y coordinates and Width,Height values
com.aspose.ocr.IRecognitionBlock block = com.aspose.ocr.RecognitionBlock.createTextBlock(6, 9, 120, 129);

// Set the Whitelist property by specifying a new block whitelist
block.setWhitelist(new char[] { '0', '1', '2', '3', '4', '5', '6', '7', '8', '9' });

// YOU CAN ADD MORE TEXT BLOCK AND SET WHITE LISTS.

// Set different configurations and add recognition block(s)
engine.getConfig().clearRecognitionBlocks();
engine.getConfig().addRecognitionBlock(block);
engine.getConfig().setDetectTextRegions(false);

// Call OcrEngine.Process method to perform OCR operation
if (engine.process())
{
    // Display the recognized text from each Page
    System.out.println(engine.getText());
} 
```

Please review the release notes of [Aspose.OCR for Java 16.10][2] for a complete view of new enhancements.

## Aspose.OCR for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for Java API][3].
*   [Download Aspose.OCR for Java][4].
*   [Aspose.OCR for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png "Aspose.OCR for Java logo"
[2]: https://docs.aspose.com/display/ocrnet/Home
[3]: https://www.aspose.com/products/ocr/java
[4]: https://downloads.aspose.com/ocr/java
[5]: https://docs.aspose.com/display/OCRJAVA/Home
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-Java
[9]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx




