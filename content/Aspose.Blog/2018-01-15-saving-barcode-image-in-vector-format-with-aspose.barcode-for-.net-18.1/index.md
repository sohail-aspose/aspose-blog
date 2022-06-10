---
title: 'Save Barcode Image In Vector Format in C# using Aspose.BarCode for .NET 18.1'
date: Mon, 15 Jan 2018 05:15:28 +0000
draft: false
url: /2018/01/15/saving-barcode-image-in-vector-format-with-aspose.barcode-for-.net-18.1/
author: Ikram Haq
summary: ''
tags: ['Generate Barcodes in Vector Image Format']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="Aspose.Barcode for .NET">}}


We are pleased to announce the release of [Aspose.Barcode for .NET][1] 18.1. The major development in this release is the support to save the generated barcode image in Vector format. This release also supports the enhanced process of drawing barcode text when the font is specified in the code snippet. Improved working of CodeLocation property has also been incorporated in this release.

## Save Barcodes in Vector Image Format

Aspose.BarCode supports the functionality to save the generated barcode image in vector format. Two new values EMF and SVG has been introduced in Aspose.BarCode.BarCodeImageFormat enumeration which can be set before saving barcode image. Aspose.BarCode.BarCodeImageFormat enumeration now contains:

*   Bmp
*   Gif
*   Jpeg
*   Png
*   Tiff
*   TiffInCmyk
*   Emf
*   Svg

How a developer can save barcode image in vector format is quite simple and is demonstrated in the code snippet given below. The code snippet contains comments that make it self explanatory.

```
// Instantiate BarCodeBuilder object
Aspose.BarCode.BarCodeBuilder builder = new Aspose.BarCode.BarCodeBuilder();

// Set the Code text for the barcode
builder.CodeText = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

// Set the symbology type to Code128
builder.EncodeType = Aspose.BarCode.Generation.EncodeTypes.Code128;

//Save the image
builder.Save("code128.svg", Aspose.BarCode.BarCodeImageFormat.Svg);
```

## Other Improvements

This release also fixes exceptions that were reported by our valued customers. The complete list of fixes in this release is as follows.

*   It was noticed that when the font is specified while saving the barcode image in vector format. The barcode inaccurate text was displayed. The process of drawing the barcode text has been improved.
*   Setting big text size with StringAlignment.Far option, it was noticed that the barcode text disappears. Now the issue has been fixed.
*   Working with CodeLocation property has been improved.

To view a complete list of enhancements and fixes, please visit the [release notes][2] page. This release also includes many important API and Backward Incompatible changes. The list of all such changes is worth seeing and can be view on the release notes page. You can access **Aspose.Barcode for .NET 18.1** through [NuGet Gallery][3].

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   [Aspose.BarCode for .NET Wiki docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+18.1+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.BarCode/
[4]: https://products.aspose.com/barcode/net
[5]: https://www.nuget.org/packages/Aspose.BarCode/
[6]: https://docs.aspose.com/display/barcodenet/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




