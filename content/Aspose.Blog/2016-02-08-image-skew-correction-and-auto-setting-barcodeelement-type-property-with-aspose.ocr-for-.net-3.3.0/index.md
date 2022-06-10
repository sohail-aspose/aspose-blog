---
title: 'Enable Automatic Image Skew Correction and BarcodeElement Type with Aspose.OCR for .Net 3.3.0'
date: Mon, 08 Feb 2016 19:28:49 +0000
draft: false
url: /2016/02/08/image-skew-correction-and-auto-setting-barcodeelement-type-property-with-aspose.ocr-for-.net-3.3.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce the release of Aspose.OCR for .NET 3.3.0. This release includes automatic and manual image skew correction in OMR template editor. The [image skew correction using the algorithm][1] has also been incorporated in this release.

## No need to set BarcodeElement type property

OMR template editor now includes support to automatically detect type of BarcodeElement symbology. Select BarcodeElement and place it on the template. Right click on the element will show the shortcut menu. Select the Detect barcode type menu option. Selecting this option will automatically detect the type of underlaying barcode and auto set the Type property of the BarcodeElement in the Properties window.



{{< figure align=center src="images/Detect_Barcode_type.jpg" alt="">}}


## Enable automatic image skew correction

Automatic and manual image skew correction can be performed while importing a scanned sheet image into the template editor.

To enable automatic image skew correction while importing scanned sheet:

*   Launch the OMR template editor.
*   Open the Settings property window by accessing the Edit menu and then Settings sub-menu.
*   Select the OmrFeatures tab and check Enable Automatic Skew Correction option.

In case, the automatic skew correction option is not enabled and you want to perform skew correction on the scanned sheet image that you have imported into the template editor, click the Deskew image icon.

## Image Skew Correction Using Algorithm

Aspose.OCR for .Net provides facility to perform image skew correction through code using the algorithm. Following is the code demonstration of how an OMR scanned sheet image can be deskewed/straighten using the SkewCorrectionAlgorithm class.

```
// Load image
OmrImage image = OmrImage.Load("sample.jpg");

// Area of the image to be processed
Rectangle area = new Rectangle(0, 0, image.Width, image.Height);

// Grayscale conversion
GrayscaleAlgorithm gs = new GrayscaleAlgorithm();
gs.Process(image, area);

// Binarization
AverageThresholdAlgorithm threshold = new AverageThresholdAlgorithm();
threshold.Process(image, area);

// Skew correction
SkewCorrectionAlgorithm skewCorrection = new SkewCorrectionAlgorithm();
skewCorrection.Process(ref image, area);

// save image
image.AsBitmap().Save("result.jpg");
```

Please review the release notes of [Aspose.OCR for .NET 3.3.0][2] for a complete list of new features & enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you check the Public API Changes section to know what has been changed since your current revision of the API.

## Aspose.OCR for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for .Net API][3].
*   [Download Aspose.OCR for .NET][4].
*   [Aspose.OCR for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://docs.aspose.com/display/ocrnet/Home
[2]: https://downloads.aspose.com/ocr/net
[3]: https://www.aspose.com/products/ocr/net
[4]: https://downloads.aspose.com/ocr/net
[5]: https://docs.aspose.com/display/ocrnet/Home
[6]: https://forum.aspose.com/c/ocr
[7]: https://blog.aspose.com/category/aspose-products/aspose-ocr-product-family/
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-.NET
[9]: http://forum.aspose.com




