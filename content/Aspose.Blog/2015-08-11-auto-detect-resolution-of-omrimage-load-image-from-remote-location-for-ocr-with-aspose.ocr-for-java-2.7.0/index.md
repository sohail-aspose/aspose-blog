---
title: 'Auto Detect Resolution of OmrImage &amp; Load Image from Remote Location for OCR with Aspose.OCR for Java 2.7.0'
date: Tue, 11 Aug 2015 07:21:49 +0000
draft: false
url: /2015/08/11/auto-detect-resolution-of-omrimage-load-image-from-remote-location-for-ocr-with-aspose.ocr-for-java-2.7.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png) We are pleased to announce that Aspose.OCR for Java 2.7.0 is now available for public use. This release includes a new OmrImage property to auto detect the image resolution of the OMR scanned image along with the means to load the image from remote location to perform OCR operation. Please review the release notes of [Aspose.OCR for Java 2.7.0][2] for a complete view of new features & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

## Auto Detect the Resolution of OmrImage

Aspose.OCR for Java now provides the OmrImage.setAutoDetectResolution property to auto detect the resolution of the scanned image to perform OMR operation. The OmrEngine tries to compare the resolution detected for the scanned image with the resolution of the OMR template. If they do not match with a slight tolerance, the OmrEngine generates an exception.

The following code snippet demonstrates how to use the newly exposed property to auto detect the image resolution.

```
 //Load the image to be analyzed
OmrImage image = OmrImage.load("sample.jpg");

//Set the auto image resolution detection property
image.setAutoDetectResolution(true);

//Load template file
OmrTemplate template = OmrTemplate.Load("sample.amr");

// Instantiate the recognition engine for the template
OmrEngine engine = new OmrEngine(template);

// Extract data. This template has only one page.
OmrProcessingResult result = engine.extractData(new OmrImage[] { image });

//Do Processing 
```

## Load Image from Remote Location (URL)

Aspose.OCR for Java provides facility to perform OCR operation on remote images as well as local ones. You just need to supply the URL of the image to newly exposed fromUrl method for the ImageStream class. Following is the simple code snippet demonstrating the usage of the said method to perform OCR on a remote image.

```
 //Initialize an instance of OcrEngine
OcrEngine ocrEngine = new OcrEngine();

//Set the Image property by loading the image from remote location
ocrEngine.setImage(ImageStream.fromUrl("http://www.someplace.com/images/sample.bmp"));

//Do Processing 
```

## Enhancements

This release has incorporated some enhancements. The list of enhancements is given below:

*   The OmrEngine can now take care of low resolution scanned images to perform OMR operation.
*   Improved OMR algorithm for better handling of OMR's GridElement & marks filled with pencil.
*   DetectTextRegions property work in the correct way i.e. if you set this property to TRUE. It will ignore the manually set text recognition block.

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
[2]: http://www.aspose.com/community/files/72/java-components/aspose.ocr-for-java/entry647030.aspx
[3]: https://www.aspose.com/products/ocr/java
[4]: https://downloads.aspose.com/ocr/java
[5]: https://docs.aspose.com/display/OCRJAVA/Home
[6]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-Java
[9]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx




