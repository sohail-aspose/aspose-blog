---
title: '.NET OCR API - Metered Licensing Support'
date: Tue, 10 Jan 2017 09:05:25 +0000
draft: false
url: /2017/01/10/metered-licensing-support-omr-aspose.ocr-.net-16.12/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

We are pleased to announce the release of [Aspose.OCR for .NET][1] 16.12. The major development in this release is support for the metered license mechanism for OMR operations. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. Furthermore overall performance of the API has also been improved in this release.

## Metered License Support for OMR Operations

Aspose.OCR for .Net provides the functionality to use metered licensing mechanism for OMR operations. We have introduced Metered class in API to accomplish this job. The following sample code will demonstrate, how to calculate the consumed OMR API requests.

```
// Create an instance of OCR Metered class
Aspose.OCR.Metered metered = new Aspose.OCR.Metered();

// Access the setMeteredKey property and pass public and private keys as parameters
metered.SetMeteredKey("*****", "*****");

// set up engine
//OmrEngine omr = new OmrEngine(new OmrTemplate());
//ocr.Image = ImageStream.FromFile(@"abc.jpg");

// do processing
// string path = "sampleimage.png";
// OmrImage omrImage = OmrImage.Load(path);

// get metered data amount
decimal amount = Aspose.BarCode.Metered.GetConsumptionQuantity();

// Display information
Console.WriteLine("Amount Consumed : " + amount.ToString());
```

## Enhancements

The following enhancements have been introduced in this release.

*   Processing of distorted images has been improved.
*   Mechanism of applying filters on the supplied image has been improved.

Please check the release notes of [Aspose.OCR for .NET 16.12][2] for a complete list of enhancements.

## Aspose.OCR for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for .NET API][3].
*   [Download Aspose.OCR for .NET][4].
*   [Aspose.OCR for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.



[1]: https://products.aspose.com/ocr/net
[2]: https://products.aspose.com/ocr/net
[3]: https://www.aspose.com/products/ocr/net
[4]: https://downloads.aspose.com/ocr/net
[5]: https://docs.aspose.com/display/ocrnet/Home
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[9]: http://forum.aspose.com




