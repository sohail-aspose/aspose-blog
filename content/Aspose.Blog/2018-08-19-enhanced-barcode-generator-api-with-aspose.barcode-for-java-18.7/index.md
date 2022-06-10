---
title: 'Use the Enhanced Barcode Generator API for Java'
date: Sun, 19 Aug 2018 17:56:35 +0000
draft: false
url: /2018/08/19/enhanced-barcode-generator-api-with-aspose.barcode-for-java-18.7/
author: Kashif Iqbal
summary: ''
tags: ['Generate Barcodes using Java', 'Java Barcode Generator API']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for Java 18.7][1]. This new version of API introduces a more powerful API for Barcode generation. It gives you more power for generating Barcodes with the desired information. For a detailed note on what is new and fixed, please visit the [release notes][2] information of API documentation.

## New Barcode Generation API

Starting from Aspose.BarCode for Java 18.7, this release introduces a new Barcode generation API. The new API, represented by BarCodeGenerator class, is simple but powerful enough to give maximum control over Barcode generation as per requirements. With this enhanced API as compared to the previous version of API i.e. BarCodeBuilder, you can generate and work with barcodes in more flexible ways.

## Characteristics of New Barcode Generation Methodology

The new Barcode generation API, BarCodeGenerator, will replace the older BarcodeBuilder with subsequent versions. Salient features of this new Barcode generation class are as follow:

*   **Generation of Barcode with Restricted Barcode Size** – If you have restricted requirements of barcode size, then you can set AutoSizeMode to Nearest and required barcode size. Barcode generator will calculate all other parameters like xDimension, AspectRatio, etc to fit barcode into the desired size.
*   **Generating Barcode without Restricted Barcode Size** – if you don’t have required size of Barcode to be generated, you can set AutoSizeMode to None and set all generator parameters by yourself
*   **Getting Generated Barcode Size** – if you just want to know the barcode size without saving the image you can call method RecalculateValues() and get barcode size
*   **Units based Barcode Generation** – All measurement values can be got and set in pixels, millimeters, inches at the same time. You can easily change the resolution of the image and prepare the same barcode for printing, LCD screens, or retina-displays.
*   **Grouping Properties by Barcode Type** – Properties for specific barcode types are grouped. Such specific properties like QR\_EncodeType of DataMatrix\_Ecc are grouped by type to simplify all the API for new users.
*   **Getting Default Text for Generated Barcode** – BarCodeGenerator has predefined default codetext, so you can just explore the default codetext format for the specific type.

For detailed code samples of this new Barcode generator class, please visit the [Generating Barcode using BarcodeGenerator][3] article of API documentation.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java][4]
*   [Download Aspose.BarCode for Java][5] – Install Aspose.BarCode for Java from Maven
*   [Aspose.BarCode for Java Wiki docs][6] – help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/18.7
[2]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Java+18.7+Release+Notes
[3]: https://docs.aspose.com/display/barcodejava/Generating+BarCode+using+New+BarCode+Generation+API
[4]: https://products.aspose.com/barcode/java
[5]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/
[6]: https://docs.aspose.com/display/barcodejava/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




