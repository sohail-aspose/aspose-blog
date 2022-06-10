---
title: 'Handle Exceptions with Aspose.OCR for Java 2.8.0'
date: Thu, 08 Oct 2015 09:19:47 +0000
draft: false
url: /2015/10/08/handle-exceptions-with-aspose.ocr-for-java-2.8.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-Java_100.png" alt="Aspose.OCR for Java logo">}}


We are pleased to announce that [Aspose.OCR for Java][1] 2.8.0 is now available for public use. This release includes exception handling to capture failures caused by the OmrEngine and getting correct multi-selected values from Grid element.

## Handling Exceptions for OmrEngine

This release of the Aspose.OCR for Java API has exposed com.aspose.omr.OmrException class along with it’s supporting methods that allow you to handle exceptions caused by OmrEngine during the processing of OMR forms.

Simple usage scenario of OmrException class is as follow

```
//Enclose your code in a try catch structure
try
{
     //Create an instance of OmrTemplate and load the .amr file
     OmrTemplate template = OmrTemplate.load("template1.amr");

     //Create an instance of OmrImage and load the scanned form
     OmrImage image = OmrImage.load("image1.png");

     //Create an instance of OmrEngine and initialize it with OmrTemplate
     OmrEngine engine = new OmrEngine(template);

     //Process the OMR form
     OmrProcessingResult result = engine.extractData(new OmrImage[]{image});
}
//Handle exceptions
catch (OmrException e)
{
    e.printStackTrace();
}
catch (IOException e)
{
    e.printStackTrace();
}
```

## Enhancements

This release has incorporated some enhancements. The list of enhancements is given below:

*   Fixed: Getting multi selected values from Grid element.
*   Fixed: Incorrect recognized text for specific file.
*   Fixed: OCR Engine hangs while performing OCR on Image of 2479 X 3508 with graphics.
*   Fixed: Arithmetic operation resulted in an overflow.

Please review the release notes of [Aspose.OCR for Java 2.8.0][2] for a complete view of new features & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

## Aspose.OCR for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for Java API][3].
*   [Download Aspose.OCR for Java][4].
*   [Aspose.OCR for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://products.aspose.com/ocr/java
[2]: https://downloads.aspose.com/ocr/java
[3]: https://products.aspose.com/ocr/java
[4]: https://downloads.aspose.com/ocr/java
[5]: https://docs.aspose.com/ocr/java/
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-Java
[9]: http://forum.aspose.com




