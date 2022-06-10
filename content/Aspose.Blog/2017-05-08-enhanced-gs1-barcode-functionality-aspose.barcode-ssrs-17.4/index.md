---
title: 'Enhanced GS1 Barcode Functionality With Aspose.BarCode for SSRS 17.4'
date: Mon, 08 May 2017 17:18:50 +0000
draft: false
url: /2017/05/08/enhanced-gs1-barcode-functionality-aspose.barcode-ssrs-17.4/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of Aspose.BarCode for Reporting Services 17.4. The major development in this release is the enhanced functionality of GS1 coded barcode. More often it is seem that GS1 code text contains complex combination of digits and letters. With Aspose.BarCode for SSRS 17.4, parsing and validation of those complex combinations is possible.

## Enhanced GS1 Barcode Generation And Recognition

Aspose.BarCode for SSRS allows developers to generate GS1 coded barcode according to AI **(Application Identifier)** specifications. New validators have been incorporated that can validate text code having only digits and complex AIs (combination of digits & letters). API will throw an exception in case it fails to validate. According to AI specification (ref: 703 AI, with letters – 324a, with more than 4 symbols) code text **“(703)123”** is incorrect. Aspose.BarCode will throw following exception if user tries to generate the barcode with **EncodeTypes** as **GS1Code128**. The following exception message will be displayed for such an incorrect barcode.

### Exception Message:

Wrong format of GS1 Code128 input string.

Checksum calculation and validation for such and many more AI specifications have been implemented.

## Enhancements

This month’s release also includes few bug fixes that were reported by our customers in the previous release. Details about these fixes are listed below.

*   Functionality of ExportToXml method has been improved. ExportToXml method now export dimension properties along with other properties of the newly define barcode into XML file.

To view the complete list of new features and fixes, please visit the [release notes][1] page. You can download the latest version by visiting the [Aspose.BarCode for Reporting Services 17.04][2] page in downloads section.

## Aspose.BarCode for Reporting Services Resources

The following resources will help you work with Aspose.BarCode for SSRS:

*   [Homepage for Aspose.BarCode for SSRS API][3]
*   [Download Aspose.BarCode for SSRS][4]
*   [Aspose.BarCode for SSRS Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://docs.aspose.com/display/barcodereportingservices/Aspose.BarCode+for+Reporting+Services+17.4+Release+Notes
[2]: http://www.aspose.com/downloads/barcode/reportingservices
[3]: https://www.aspose.com/products/barcode/reporting-services
[4]: https://downloads.aspose.com/barcode/reportingservices
[5]: https://docs.aspose.com/display/barcodereportingservices/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




