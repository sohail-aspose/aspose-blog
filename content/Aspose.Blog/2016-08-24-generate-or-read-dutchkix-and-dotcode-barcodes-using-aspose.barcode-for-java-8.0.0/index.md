---
title: 'Generate and Read DutchKix and DotCode Barcodes using Java'
date: Wed, 24 Aug 2016 16:46:53 +0000
draft: false
url: /2016/08/24/generate-or-read-dutchkix-and-dotcode-barcodes-using-aspose.barcode-for-java-8.0.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="Aspose.BarCode for Java logo">}}


We are pleased to announce the release of Aspose.Barcode for Java 8.0.0. This release supports generating/reading DutchKix and DotCode barcode types. Several new enhancements have also been made in the barcode recognition algorithm to further improve the recognition process while reading barcodes from poor quality QR, Code128, DataMatrix, and Aztec codes.

## Generate DutchKix or DotCode Barcodes using Java

Aspose.Barcode for Java allows you to generate DutchKix or DotCode barcodes. You can set **SymbologyType** to **DutchKix** or **DotCode** to generate these barcodes. Following is the code demonstration.

```
// Create an instance of BarCodeBuilder class and pass parameters
// 1. Code Text
// 2. BarCode Symbology - DotCode
com.aspose.barcode.BarCodeBuilder builder = 
                new com.aspose.barcode.BarCodeBuilder("!AA-11;", com.aspose.barcode.Symbology.DotCode);

// Call save method to save the barcode in image format
builder.save("DotCode.png");

////////////////////////////////////////////////////////////////////////////

// Create an instance of BarCodeBuilder class and pass parameters
// 1. Code Text
// 2. BarCode Symbology - DutchKIX
com.aspose.barcode.BarCodeBuilder builder = 
                new com.aspose.barcode.BarCodeBuilder("!AA-11;", com.aspose.barcode.Symbology.DutchKIX);

// Call save method to save the barcode in image format
builder.save("DutchKIX.png");
```

## Enhancements

The following is a list of improvements included in this release.

*   Improve the algorithm to read barcodes even if the image is not rotated.
*   Improve algorithm to Read the barcodes from a PNG image having 100 multiple barcodes in it.
*   Improve algorithm to detect the barcodes with default settings.
*   Support recognition of invasion in the quiet zone for a data matrix.
*   Improve 3D-distorted Aztec code recognition.
*   Improve recognition of the Aztec code.
*   Recognize poor quality code128 with histogram method.
*   Fix the issue with Rows property for PDF417 barcode.
*   Investigate and fix order of recognizing barcodes.
*   Improve DotCode regions recognition.
*   Read the corrupted QR barcode.

To view a complete list of new features and fixes and to download the latest release, please visit Aspose.Barcode for Java 8.0.0 page in the downloads section.

## Aspose.BarCode for Java Resources

The resources you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][1]
*   [Download Aspose.BarCode for Java][2]
*   [Aspose.BarCode for Java Wiki docs][3] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][6] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.aspose.com/products/barcode/java
[2]: https://downloads.aspose.com/barcode/java
[3]: https://docs.aspose.com/display/barcodejava/Home
[4]: https://forum.aspose.com/c/barcode
[5]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[6]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




