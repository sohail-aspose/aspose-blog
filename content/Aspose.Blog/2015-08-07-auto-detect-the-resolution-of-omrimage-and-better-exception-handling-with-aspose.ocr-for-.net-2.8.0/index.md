---
title: 'Auto Detect the Resolution of OmrImage and Better Exception Handling with Aspose.OCR for .Net 2.8.0'
date: Fri, 07 Aug 2015 13:36:26 +0000
draft: false
url: /2015/08/07/auto-detect-the-resolution-of-omrimage-and-better-exception-handling-with-aspose.ocr-for-.net-2.8.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-net_100.png) We are pleased to announce that Aspose.OCR for .NET 2.8.0 is now available for public use. This release includes exception handling to capture failures caused by the OmrEngine and a new OmrImage property to auto detect the image resolution of the OMR scanned image. Please review the release notes of [Aspose.OCR for .NET 2.8.0][2] for a complete view of new feature & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

## Auto Detect the Resolution of OmrImage

Aspose.OCR for .Net now provides the OmrImage.AutoDetectResolution property to auto detect the resolution of the scanned image to perform OMR operation. The OmrEngine tries to compare the resolution detected for the scanned image with the resolution of the OMR template. If they do not match with a slight tolerance, the OmrEngine generates an exception.

The following code snippet demonstrates how to use the newly exposed property to auto detect the image resolution.

```
 //Load the image to be analyzed
OmrImage image = OmrImage.Load("sample.jpg");

//Set the auto image resolution detection property
image.AutoDetectResolution = true;

//Load template file
OmrTemplate template = OmrTemplate.Load("sample.amr");

//Instantiate the recognition engine for the template
OmrEngine engine = new OmrEngine(template);

//Extract data
OmrProcessingResult result = engine.ExtractData(new OmrImage[] { image });

//Do Processing 
```

## Exception Handling for OmrEngine

This release of the Aspose.OCR for .NET API has exposed the Aspose.OMR.OmrException class along with it's supporting methods that allows to handle the exceptions caused by the OmrEngine during the processing of OMR forms.

Simple usage scenario of OmrException class is as follow

```
 //Enclose your code in a try catch structure
try
{
   //Create an instance of OmrTemplate and load the .amr file
   OmrTemplate template = OmrTemplate.Load("sample.amr");

   //Create an instance of OmrImage and load the scanned form
   OmrImage image = OmrImage.Load(imageName);

   //Create an instance of OmrEngine and initialize it with OmrTemplate
   OmrEngine engine = new OmrEngine(template);

   //Process the OMR form
   OmrProcessingResult result = engine.ExtractData(new OmrImage[] { image });
}
//Handle exceptions
catch (OmrException e)
{
   Console.WriteLine(e.StackTrace);
} 
```

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
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/entry646206.aspx
[3]: https://www.aspose.com/products/ocr/net
[4]: https://downloads.aspose.com/ocr/net
[5]: https://docs.aspose.com/display/ocrnet/Home
[6]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[9]: https://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx




