---
title: 'Optimize recognition and process noisy OMR scanned sheet images by setting setSavePreprocessedImages property to false with Aspose.OCR for Java 3.0.0'
date: Wed, 02 Dec 2015 08:20:58 +0000
draft: false
url: /2015/12/02/optimize-recognition-and-process-noisy-omr-scanned-sheet-images-by-setting-setsavepreprocessedimages-property-to-false-with-aspose.ocr-for-java-3.0.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png) We are pleased to announce that Aspose.OCR for Java 3.0.0 is now available for public use. This release includes optimizing OCR process by setting not to save preprocessed images and improvements in the algorithms to process the noisy OMR scanned sheet images.

## Exclude Preprocessed Images from OCR operation

Aspose.OCR for Java provides facility to exclude preprocessed images from being saved during OCR operation. This functionality can be achieved by setting the setSavePreprocessedImages property of the configuration \[OCRConfig\] class to true.

Following is the simple code snippet demonstrating the usage of the said property to optimize the OCR process.

```
 String FileName = "";

//Initialize an instance of OcrEngine
OcrEngine ocr = new OcrEngine();                        

//Set the Image property by loading the image from file path location
ocr.setImage(ImageStream.fromFile(FileName));

// Set the SavePreprocessedImages property to false
ocr.getConfig().setSavePreprocessedImages(false);        

if (ocr.process())
{
      // Do processing
} 
```

Please review the release notes of [Aspose.OCR for Java 3.0.0][2] for a complete view of new features. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

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




