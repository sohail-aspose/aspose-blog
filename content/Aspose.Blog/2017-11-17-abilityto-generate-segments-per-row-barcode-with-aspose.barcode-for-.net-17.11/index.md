---
title: 'Generate Segments Per Row Barcode in SQL Server Reporting Services'
date: Fri, 17 Nov 2017 03:58:34 +0000
draft: false
url: /2017/11/17/abilityto-generate-segments-per-row-barcode-with-aspose.barcode-for-.net-17.11/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of [Aspose.BarCode for Reporting Services][1] 17.11. The major development in this release is the support to generate databar coded barcode with segments per row.

## Barcode Segments Per Row

Aspose.BarCode for Reporting Services now enables the developers to generate databar coded barcode with segments per row. Generating segments per row for a databar is very simple and is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

```
 //Instantiate BarCodeBuilder object
Aspose.BarCode.BarCodeBuilder builder = new Aspose.BarCode.BarCodeBuilder();

//Set the Code text for the barcode
builder.CodeText = "(01)98898765432106(3202)012345(15)991231";

//Set the symbology type to Code128
builder.EncodeType = Aspose.BarCode.Generation.EncodeTypes.DatabarExpandedStacked;

//Set the cloumn property to define segments per row
builder.Columns = 6;

//Save the image
builder.Save("6segmets.png"); 
```

To view the complete list of new features and fixes, please visit the [release notes][2] page. This release also includes many important API and Backward Incompatible changes. The list of all such changes are worth seeing and can be view on release notes page. You can download the latest version by visiting the [Aspose.BarCode for Reporting Services 17.11][3] page in downloads section.

## Aspose.BarCode for Reporting Services Resources

The following resources will help you work with Aspose.BarCode for SSRS:

*   [Homepage for Aspose.BarCode for SSRS API][4]
*   [Download Aspose.BarCode for SSRS][5]
*   [Aspose.BarCode for SSRS docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://products.aspose.com/barcode/reporting-services
[2]: https://docs.aspose.com/barcode/reportingservices/aspose-barcode-for-reporting-services-17-11-release-notes/
[3]: https://downloads.aspose.com/barcode/reportingservices
[4]: https://products.aspose.com/barcode/reportingservices
[5]: https://downloads.aspose.com/barcode/reportingservices
[6]: https://docs.aspose.com/barcode/reportingservices
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




