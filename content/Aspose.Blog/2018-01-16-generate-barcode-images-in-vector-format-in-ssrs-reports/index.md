---
title: 'Set Vector Format of Barcode Image using Aspose.BarCode for SSRS 18.1'
date: Tue, 16 Jan 2018 03:56:17 +0000
draft: false
url: /2018/01/16/generate-barcode-images-in-vector-format-in-ssrs-reports/
author: Ikram Haq
summary: ''
tags: ['Embed barcode in vector image format in SSRS', 'Generate barcode images in vector format SSRS']
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of [Aspose.BarCode for Reporting Services][1] 18.1. The major development in this release is the support of the generated barcode image in Vector format.

## Setting Vector Format Of Barcode Image

Aspose.BarCode for Reporting Services now enables the developers to save the generated barcode image in vector format. Two new formats EMF and SVG have been introduced. Saving the barcode image in vector format is very simple and is demonstrated in the code snippet given below. The code snippet contains comments that make it self explanatory.

```
// Instantiate BarCodeBuilder object
Aspose.BarCode.ReportingServices.BarCodeBuilder builder = new Aspose.BarCode.ReportingServices.BarCodeBuilder();

// Set the Code text for the barcode
builder.CodeText = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

// Set the symbology type to QR
builder.EncodeType = Aspose.BarCode.Generation.EncodeTypes.Code128;

//Save the image
builder.Save("code128.svg", Aspose.BarCode.ReportingServices.BarCodeImageFormat.Svg);
```

## Other Improvements

This release also fixes exceptions that were reported by our valued customers. The complete list of fixes in this release is as follows.

*   It was noticed that when font is specified while saving the barcode image in vector format. The barcode inaccurate text was displayed. The process of drawing barcode text has been improved.
*   Setting big text size with StringAlignment.Far option, it was noticed that the barcode text disappears. Now the issue has been fixed.
*   Working of CodeLocation property has been improved.

To view the complete list of new features and fixes, please visit the [release notes][2] page. This release also includes many important API and Backward Incompatible changes. The list of all such changes is worth seeing and can be view on the release notes page. You can download the latest version by visiting the [Aspose.BarCode for Reporting Services 18.1][3] page in the downloads section.

## Aspose.BarCode for Reporting Services Resources

The following resources will help you work with Aspose.BarCode for SSRS:

*   [Homepage for Aspose.BarCode for SSRS API][4]
*   [Download Aspose.BarCode for SSRS][5]
*   [Aspose.BarCode for SSRS Wiki docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://products.aspose.com/barcode/reporting-services
[2]: https://docs.aspose.com/display/barcodereportingservices/Aspose.BarCode+for+Reporting+Services+18.1+Release+Notes
[3]: http://downloads.aspose.com/barcode/reportingservices
[4]: https://products.aspose.com/barcode/reporting-services
[5]: https://downloads.aspose.com/barcode/reportingservices
[6]: https://docs.aspose.com/display/barcodereportingservices/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




