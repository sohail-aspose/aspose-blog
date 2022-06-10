---
title: 'Set Version Number in QR Barcode in SSRS'
date: Tue, 12 Dec 2017 05:08:50 +0000
draft: false
url: /2017/12/12/version-number-setting-in-qr-coded-barcode-with-aspose.barcode-for-ssrs-17.12/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of Aspose.BarCode for Reporting Services 17.12. The major development in this release is the support to generate QR coded barcode with setting version number.

## Set Version Number for QR Barcodes

Aspose.BarCode for Reporting Services now enables the developers to generate QR coded barcode with setting its version number. Setting QR version number is very simple and is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

```
// Instantiate BarCodeBuilder object
Aspose.BarCode.BarCodeBuilder builder = new Aspose.BarCode.BarCodeBuilder();

// Set the Code text for the barcode
builder.CodeText = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

// Set the symbology type to QR
builder.EncodeType = Aspose.BarCode.Generation.EncodeTypes.QR;

// Set the error level
builder.QRErrorLevel = Aspose.BarCode.QRErrorLevel.LevelQ;

// Set the QR barcode version number
builder.QRVersion = Aspose.BarCode.QRVersion.Version10;

//Save the image
builder.Save("qr\_version10\_errorQ.png");

```

## Other Improvements

This release also fixes exceptions that were reported by our valued customers. The complete list of fixes in this release is as follows.

*   The process of setting a license has been improved. Now API will show the correct exception message in case the license subscription is expired. Setting license time has also been improved.
*   Working of Aspose.BarCode in a multi-threaded environment has been enhanced.
*   The databarStacked barcode recognition process has been enhanced.

To view the complete list of new features and fixes, please visit the [release notes][1] page. This release also includes many important API and Backward Incompatible changes. The list of all such changes is worth seeing and can be view on the release notes page. You can download the latest version by visiting the Aspose.BarCode for Reporting Services 17.12 page in the downloads section.

## Aspose.BarCode for Reporting Services Resources

The following resources will help you work with Aspose.BarCode for SSRS:

*   [Homepage for Aspose.BarCode for SSRS API][2]
*   [Download Aspose.BarCode for SSRS][3]
*   [Aspose.BarCode for SSRS Wiki docs][4] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][6] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://docs.aspose.com/display/barcodereportingservices/Aspose.BarCode+for+Reporting+Services+17.12+Release+Notes
[2]: https://www.aspose.com/products/barcode/reporting-services
[3]: https://downloads.aspose.com/barcode/reportingservices
[4]: https://docs.aspose.com/display/barcodereportingservices/Home
[5]: https://forum.aspose.com/c/barcode
[6]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




