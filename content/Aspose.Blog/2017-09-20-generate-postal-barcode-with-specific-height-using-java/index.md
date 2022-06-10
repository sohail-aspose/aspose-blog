---
title: 'Generate Postal Barcode with Specific Height using Java'
date: Wed, 20 Sep 2017 18:56:29 +0000
draft: false
url: /2017/09/20/generate-postal-barcode-with-specific-height-using-java/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of [Aspose.Barcode for Java][1] 17.8. Aspose.BarCode versions brefore 17.8, it was not possible to set the barcode bar's height while generating Postal barcodes like postnet, AustraliaPost etc. The major development in this release is the support to generate the postal barcode with specified height. The functionality to recognize GS1Code128 coded barcode has also been improved in this release.

## Postal Barcode Generation With Specific Height in Java

Previous versions of Aspose.BarCode, it was not possible to set the height of bars of Postal barcodes like Postnet, AustraliaPost, Planet, OneCode and RM4SCC. Aspose.Barcode for .NET 17.8 now allows developers to set the bar height. The said functionality is illustrated in the following code sample.

```
String codeText = "12345678";

// Create an instance of BarCodeBuilder class
BarCodeBuilder barCodeBuilder = new BarCodeBuilder();

// Set barcode text
barCodeBuilder.setCodeText(codeText);

// Set encoding type
BaseEncodeType encodeType = EncodeTypes.POSTNET;
barCodeBuilder.setEncodeType(encodeType);

// Set barcode Dimension and height
barCodeBuilder.setxDimension(1f);
barCodeBuilder.setBarHeight(40);

// Save the barcode image
barCodeBuilder.save("postnet.png"); 
```

## Other Improvements

In addition to above, this release also fixes exceptions that were reported by our valued customers. Complete list of enhancements and fixes in this release is as follows.

*   Process of GS1Code128 coded barcode recognition has been enhanced. The functionality has been improved in such a way that it now recognize correct type of GS1Code128 coded barcode.
*   Process of generating EAN14 barcode has been improved.
*   Functionality to recognize DatabarStacked coded barcode has been improved.
*   Functionality of yDimension property has been enhanced. It is now working for 2D barcodes e.g. CodablockF.

To view a complete list of new features, fixes and to download the latest release, please visit [Aspose.Barcode for Java 17.8][2] page in downloads section.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

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
[6]: http://forum.aspose.com
[7]: https://forum.aspose.com/c/barcode
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




