---
title: 'Java OCR API Supports Metered License'
date: Tue, 10 Jan 2017 10:59:19 +0000
draft: false
url: /2017/01/10/metered-licensing-support-omr-aspose.ocr-java-16.12/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

We are pleased to announce the release of [Aspose.OCR for Java][1] 16.12. The major development in this release is support for metered license mechanism for OMR operations. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. Furthermore overall performance of the API has also been improved in this release.

## Metered License Support for OMR Operations

Aspose.OCR for Java provides the functionality to use metered licensing mechanism for OMR operations. We have introduced Metered class in API to accomplish this job. The following sample code will demonstrate, how to calculate the consumed OMR API requests.

```
// set up OMR engine
        com.aspose.omr.OmrEngine omr = new com.aspose.omr.OmrEngine(new com.aspose.omr.OmrTemplate());

        // Create an instance of OCR Metered class
        com.aspose.ocr.metered.Metered metered = new com.aspose.ocr.metered.Metered();
        
        // Access the setMeteredKey property and pass public and private keys as parameters
        metered.setMeteredKey("publicKeyValue", "privateKeyValue");
 
        // Get consumed qantity value before accessing API
        double amountBefore = com.aspose.ocr.metered.Metered.getConsumptionQuantity();
        
        // do processing
        // String path = "sampleimage.png";
        // com.aspose.omr.OmrImage omrImage = com.aspose.omr.OmrImage.load(path);
 
        //Since upload data is running on another thread, so we need wait some time
        Thread.sleep(10000);
        
        // get metered data amount
        double amountAfter = com.aspose.ocr.metered.Metered.getConsumptionQuantity();
```

## Enhancements

Following enhancements have been introduced in this release.

*   Processing of distorted images has been improved.
*   Mechanism of applying filters on the supplied image has been improved.

Please review the release notes of Aspose.OCR for Java 16.12 for a complete view of new enhancements.

## Aspose.OCR for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for Java API][2].
*   [Download Aspose.OCR for Java][3].
*   [Aspose.OCR for Java online documentation][4] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][8] for a chat.




[1]: https://products.aspose.com/ocr/java
[2]: https://products.aspose.com/ocr/java
[3]: https://downloads.aspose.com/ocr/java
[4]: https://docs.aspose.com/display/OCRJAVA/Home
[5]: https://forum.aspose.com/c/ocr
[6]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[7]: https://github.com/aspose-ocr/Aspose.OCR-for-Java
[8]: http://forum.aspose.com




