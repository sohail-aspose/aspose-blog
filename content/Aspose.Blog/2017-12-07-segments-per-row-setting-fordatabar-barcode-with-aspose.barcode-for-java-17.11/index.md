---
title: 'Generate Databar Coded Barcode with Segments Per Row using Java'
date: Thu, 07 Dec 2017 17:01:07 +0000
draft: false
url: /2017/12/07/segments-per-row-setting-fordatabar-barcode-with-aspose.barcode-for-java-17.11/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

Aspose.BarCode for Java 17.11 is available for [download][1] now. The major development in this release is the support to [generate databar coded barcode with segments per row][2]. Enhanced functionality to read barcode from PDF has also been incorporated in this release.

## Generating Segments Per Row For Databar Barcode

Aspose.BarCode for Java now supports the functionality to [generate segments per row databar encoded barcode][3]. This functionality allows the developers to adjust the amount of information per (each) row in the barcode. A property BarCodeBuilder.setColumns has been introduced to define the said setting. How a developer can set segments per row for a databar is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

```
 //Instantiate BarCodeBuilder object
com.aspose.barcode.BarCodeBuilder builder = new com.aspose.barcode.BarCodeBuilder();

//Set the Code text for the barcode
builder.setCodeText("(01)98898765432106(3202)012345(15)991231"); 

//Set the symbology type to Code128
builder.setEncodeType(com.aspose.barcode.EncodeTypes.DATABAR_EXPANDED_STACKED);

//Set the cloumn property to define segments per row
builder.setColumns(6);

//Save the image
builder.save("6segmets.png"); 
```

## Other Improvements

Following is the list of improvements made in this release and bug fixes that were reported by our valued customers.

*   Functionality to recognize barcode from image has been enhanced. The functionality has been enhanced in such a way that API will extract exact number of available barcodes. No unwanted barcodes.
*   The process to extract supplement barcode has been improved. Aspose.BarCode now look for special parity pattern for correct recognition of supplement barcode.
*   DataMatrix barcode recognition process from a TIFF image has been improved. Aspose.BarCode returns all DataMatrix barcode if RecognitionMode.MaxQuality recognition mode is used.
*   Barcode recognition process have been enhanced to detect barcodes from PDF files.

To view a complete list of enhancements and fixes, please visit the [release notes][4] page.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java API][5]
*   [Download Aspose.BarCode for Java][6]
*   [Aspose.BarCode for Java Wiki docs][7] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][8] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][9] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][10] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/barcode/java
[2]: https://docs.aspose.com/barcode/java/generate-segments-per-row-barcode/
[3]: https://docs.aspose.com/barcode/java/generate-segments-per-row-barcode/
[4]: https://docs.aspose.com/barcode/java/aspose-barcode-for-java-17-11-release-notes/
[5]: https://products.aspose.com/barcode/java
[6]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-barcode/
[7]: https://docs.aspose.com/barcode/java
[8]: https://forum.aspose.com/c/barcode
[9]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[10]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




