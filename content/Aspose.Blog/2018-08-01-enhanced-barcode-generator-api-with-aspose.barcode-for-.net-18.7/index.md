---
title: 'Enhanced .NET Barcode Generator API for C# and VB.NET'
date: Wed, 01 Aug 2018 16:14:27 +0000
draft: false
url: /2018/08/01/enhanced-barcode-generator-api-with-aspose.barcode-for-.net-18.7/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Barcode for .NET 18.7][1]. From this release, we are introducing a more powerful API for Barcode generation using Aspose.Barcode. It gives you more power for generating Barcodes with the desired information. For a detailed note on what is new and fixed, please visit the [release notes][2] information of API documentation.

## New .NET Barcode Generation API

Starting from Aspose.Barcode for .NET 18.7, this month’s release introduces a new API for Barcode generation. The new API, represented by [BarcodeGenerator][3] class, is simple but powerful enough to give maximum control over Barcode generation as per requirements. With this enhanced API as compared to previous version of API i.e. BarcodeBuilder, you can generate and work with barcodes in more flexible ways.

## Characteristics of New Barcode Generation Methodology

The new Barcode generation API, BarcodeGenerator, will replace the older BarcodeBuilder with subsequent versions. Salient features of this new Barcode generation class are as follow:

*   **Generation of Barcode with Restricted Barcode Size** - If you have restricted requirements of barcode size, then you can set AutoSizeMode to Nearest and required barcode size. Barcode generator will calculate all other parameters like xDimension, AspectRatio, etc to fit barcode into the desired size.
*   **Generating Barcode without Restricted Barcode Size** - if you don’t have required size of Barcode to be generated, you can set AutoSizeMode to None and set all generator parameters by yourself
*   **Getting Generated Barcode Size** - if you just want to know the barcode size without saving the image you can call method RecalculateValues() and get barcode size
*   **Units based Barcode Generation** - All measurement values can be got and set in pixels, millimeters, inches in the same time. You can easily change the resolution of the image and prepare the same barcode for printing, LCD screens, or retina-displays.
*   **Grouping Properties by Barcode Type** \- Properties for specific barcode types are grouped. Such specific properties like QR\_EncodeType of DataMatrix\_Ecc are grouped by type to simplify all the API for new users.
*   **Getting Default Text for Generated Barcode** \- GeBarCodeGenearator has predefined default codetext, so you can just explore the default codetext format for the specific type.

For detailed code samples of this new Barcode generator class, please visit the [Generating Barcode using BarcodeGenerator][4] article of API documentation.

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][5]
*   [Download Aspose.BarCode for .NET][6]
*   [Aspose.BarCode for .NET Wiki docs][7] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][9] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.BarCode/
[2]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+18.7+Release+Notes
[3]: https://apireference.aspose.com/net/barcode/aspose.barcode.generation/barcodegenerator
[4]: https://docs.aspose.com/display/barcodenet/Generating+Barcodes+using+New+Barcode+Generation+API
[5]: https://products.aspose.com/barcode/net
[6]: https://www.nuget.org/packages/Aspose.BarCode/
[7]: https://docs.aspose.com/display/barcodenet/Home
[8]: https://forum.aspose.com/c/barcode
[9]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[10]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




