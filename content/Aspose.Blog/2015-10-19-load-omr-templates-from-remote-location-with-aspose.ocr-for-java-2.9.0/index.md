---
title: 'Load OMR Templates from Remote Location using Java'
date: Mon, 19 Oct 2015 11:14:19 +0000
draft: false
url: /2015/10/19/load-omr-templates-from-remote-location-with-aspose.ocr-for-java-2.9.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-Java_100.png" alt="Aspose.OCR for Java logo">}}


  
We are pleased to announce that [Aspose.OCR for Java][1] 2.9.0 is now available for public use. This release includes  
loading OMR templates from a remote location. Scanned sheet images can also be loaded from a remote location by using this version.

## Load OMR Template from URL using Java

Aspose.OCR for Java provides facility to load OMR template from a remote location. You just need to supply the URL of the OMR template to newly exposed loadFromUrl method.

Following is the simple code snippet demonstrating the usage of the said method to load OMR template from a remote location.

```
String templateUrl = "https://sampleurl.com/template.amr";
String imageUrl = "https://sampleurl.com/image.jpg";
        
// Initialize an instance of OmrTemplate by loading the OMR template from URL
OmrTemplate template = OmrTemplate.loadFromUrl(templateUrl);
        
// image loading from url
OmrImage image = OmrImage.loadFromUrl(imageUrl);
        
// continue working with template and image as usual
OmrEngine engine = new OmrEngine(template);
OmrProcessingResult result = engine.extractData(new OmrImage[] { image });

// Do processing
```

Please review the release notes of [Aspose.OCR for Java 2.9.0][2] for a complete view of new features. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

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
[2]: https://docs.aspose.com/ocr/java/
[3]: https://products.aspose.com/ocr/java
[4]: https://downloads.aspose.com/ocr/java
[5]: https://docs.aspose.com/ocr/java/
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-Java
[9]: http://forum.aspose.com




