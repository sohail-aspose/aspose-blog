---
title: 'Generate GS1-128 AI 8102 coupon extended and UPCA &amp; GS1 Databar coupon barcodes using Aspose.BarCode for .NET 16.10'
date: Sun, 09 Oct 2016 23:17:38 +0000
draft: false
url: /2016/10/09/generate-gs1-128-ai-8102-coupon-extended-and-upca-gs1-databar-coupon-barcodes-and-using-aspose.barcode-for-.net-16.10/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png) We are pleased to announce the release of Aspose.Barcode for .NET 16.10. This release supports generating GS1-128 AI 8102 coupon extended barcode type. This release also supports generating UPCA & GS1 Databar coupon coded barcodes. Support for setting wide narrow ratio of the bars in barcode have also been incorporated in this release.

## Generate GS1-128 AI 8102 coupon extended barcode

Aspose.Barcode for .NET allows you to generate GS1-128 AI 8102 coupon extended barcode. Following is the simple code demonstration.

```
 // Initialize BarCode builder class object
BarCodeBuilder barCodeBuilder = new BarCodeBuilder();

// Set symbology type as GS1-128 AI 8102 coupon extended and set the barcode text
barCodeBuilder.SymbologyType = Symbology.UpcaGs1Code128Coupon;

// upca part is "514141100906", GS1Code128 part is "(8102)03"
barCodeBuilder.CodeText = "514141100906(8102)03";

// save barcode
barCodeBuilder.Save("UpcaGs1Code128Coupon.png"); 
```

## Generate UPCA & GS1 Databar coupon barcode

Aspose.Barcode for .NET now supports UPCA & GS1 Databar coupon barcode. Following is the sample code demonstration.

```
 // Initialize BarCode builder class object
BarCodeBuilder barCodeBuilder = new BarCodeBuilder();

// Set symbology type as UPCA & GS1 Databar coupon and set the barcode text
barCodeBuilder.SymbologyType = Symbology.UpcaGs1DatabarCoupon;

// upca part is "514141100906", GS1Databar part is "(8110)001234502239811110555"
barCodeBuilder.CodeText = "512345678900(8110)001234502239811110555";

// set barcode caption
barCodeBuilder.CaptionAbove.Text = "012345-022398";

// save barcode
barCodeBuilder.Save("couponUpcaDatabar.png"); 
```

## Setting wide narrow ratio for bars in barcode

Using Aspose.Barcode for .NET, developers can set the wide narrow ratio of the bars in the barcode. Following is the sample code snippet to set the wide narrow ratio.

```
 // Create an instance of BarCodeBuilder class.
// Set the symbology and code text.
BarCodeBuilder barCodeBuilder = new BarCodeBuilder("blackReduction", Symbology.Code128);

// Set X dimension.
barCodeBuilder.xDimension = 1.2f;

// Set bar width reduction property
barCodeBuilder.BarWidthReduction = 0.2f;

// Save the barcode image
barCodeBuilder.Save("blackReduction.png"); 
```

## Enhancements

Following is a list of improvements included in this release.

*   Process of reading PDF417 barcode has been improved.
*   Process of reading Code93Standard barcode has been improved.
*   Process of reading datamtrix barcode has been improved.
*   Process of reading EAN13 barcode has been improved.
*   Functionality to generate QR barcode with custom height and width has been improved.
*   Functionality to generate ISSN barcode has been improved.

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for .NET 16.10 page in downloads section][2].

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[3]: https://www.aspose.com/products/barcode/net
[4]: https://downloads.aspose.com/barcode/net
[5]: https://docs.aspose.com/display/barcodenet/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




