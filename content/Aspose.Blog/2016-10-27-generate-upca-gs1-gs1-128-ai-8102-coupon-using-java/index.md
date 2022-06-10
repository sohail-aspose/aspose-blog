---
title: 'Generate UPCA, GS1, GS1-128, AI 8102 Coupon using Java'
date: Thu, 27 Oct 2016 08:59:57 +0000
draft: false
url: /2016/10/27/generate-upca-gs1-gs1-128-ai-8102-coupon-using-java/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="Aspose.BarCode for Java logo">}}


We are pleased to announce the release of [Aspose.Barcode for Java][1] 16.10. This release supports generating GS1-128 AI 8102 coupon extended barcode type. This release also supports generating UPCA & GS1 Databar coupon coded barcodes. Support for setting wide narrow ratio of the bars in barcode have also been incorporated in this release.

## Generate GS1-128 AI 8102 Coupon Extended Barcode

Aspose.Barcode for Java allows you to generate GS1-128 AI 8102 coupon extended barcode. Following is the simple code demonstration.

```
 // Initialize BarCode builder class object
com.aspose.barcode.BarCodeBuilder barCodeBuilder = new com.aspose.barcode.BarCodeBuilder();

// Set symbology type as GS1-128 AI 8102 coupon extended and set the barcode text
barCodeBuilder.setSymbologyType(com.aspose.barcode.Symbology.UpcaGs1Code128Coupon);

// upca part is "514141100906", GS1Code128 part is "(8102)03"
barCodeBuilder.setCodeText("514141100906(8102)03");

// save barcode
barCodeBuilder.save("UpcaGs1Code128Coupon.png"); 
```

## Generate UPCA & GS1 Databar Coupon Barcode

Aspose.Barcode for .NET now supports UPCA & GS1 Databar coupon barcode. Following is the sample code demonstration.

```
 // Initialize BarCode builder class object
com.aspose.barcode.BarCodeBuilder barCodeBuilder = new com.aspose.barcode.BarCodeBuilder();

// Set symbology type as UPCA & GS1 Databar coupon and set the barcode text
barCodeBuilder.setSymbologyType(com.aspose.barcode.Symbology.UpcaGs1DatabarCoupon);

// upca part is "514141100906", GS1Databar part is "(8110)001234502239811110555"
barCodeBuilder.setCodeText("512345678900(8110)001234502239811110555");

// set barcode caption
barCodeBuilder.getCaptionAbove().setText("012345-022398");

// save barcode
barCodeBuilder.save("couponUpcaDatabar.png"); 
```

## Set Wide Narrow Ratio for Bars in Barcode

Using Aspose.Barcode for .NET, developers can set the wide narrow ratio of the bars in the barcode. Following is the sample code snippet to set the wide narrow ratio.

```
 // Initialize BarCode builder class object
com.aspose.barcode.BarCodeBuilder barCodeBuilder = new com.aspose.barcode.BarCodeBuilder();

// Set symbology type as Code128 and set the barcode text
barCodeBuilder.setSymbologyType(com.aspose.barcode.Symbology.Code128);
barCodeBuilder.setCodeText("blackReduction");

// Set X dimension.
barCodeBuilder.setxDimension(1.2f);

// Set bar width reduction property
barCodeBuilder.setBarWidthReduction(0.2f);

// Save the barcode image
barCodeBuilder.save("blackReduction.png"); 
```

## Enhancements

Following is a list of improvements included in this release.

*   Process of reading PDF417 barcode has been improved.
*   Process of reading QR barcode has been improved.
*   Processing of ISSN barcodes has been improved.
*   Functionality to read EAN13 barcode has been improved.

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for Java 16.10][2] page in the downloads section.

## Aspose.BarCode for Java Resources

The resources you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][3]
*   [Download Aspose.BarCode for Java][4]
*   [Aspose.BarCode for Java Wiki docs][5] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/java
[2]: https://downloads.aspose.com/barcode/java
[3]: https://products.aspose.com/barcode/java
[4]: https://downloads.aspose.com/barcode/java
[5]: https://docs.aspose.com/barcode/java
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




