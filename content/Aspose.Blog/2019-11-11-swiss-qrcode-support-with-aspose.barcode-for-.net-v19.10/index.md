---
title: 'Generate and Read Swiss QR Code using C# - .NET Barcode Generator API'
date: Mon, 11 Nov 2019 01:38:09 +0000
draft: false
url: /2019/11/11/swiss-qrcode-support-with-aspose.barcode-for-.net-v19.10/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are glad to roll out our latest release of [Aspose.BarCode for .NET v19.10][1]/) having support for widely used Swiss QRCode. This new feature will make developers capable of developing applications to use it on bills, making digital payments, product packaging, railways, bike-sharing and even for buying bitcoins. Details of all the new exciting features can be found in the [release notes][2] containing a list of all the new added features, bugs resolution and public API changes which a developer should know for working with the latest upgrades. So let us jump into this new release and see how these new features can be used.

## Generate Swiss QR Code using C#

One of the important usages of the Swiss QR Code is to replace the previous payment slips. For this purpose, detailed information is required to trigger payments and process the QR invoice. Aspose.BarCode has provided all those necessary payment information by introducing new classes  [SwissQRBill][3] and  [SwissQRCodetext][4] which provide a large number of properties required to work with the Swiss QR Codes.

Here is a detailed example of generating the Swiss QR Code. To perform this activity you have to instantiate a  [ComplexBarcodeGenerator][5] instance and provide [SwissQRCodetext][6] containing all the necessary information for billing. The following code sample shows how to generate a Swiss QR code using C#.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageComplexBarcodes-GenerateComplexBarcodes-GenerateComplexBarcodes.cs" >}}

The following is the output Swiss QR Code generated with the above code sample:



{{< figure align=center src="images/swissQRCodetext_out.png" alt="">}}


You may visit the following link for this example and other details in the developers' guide.

*   [Generate Swiss QR Code][7]

## Read the Swiss QR Code using C#

As mentioned earlier, Swiss codes are widely used so reading is also implemented for a wide range of Swiss QR Codes. A new class [ComplexCodetextReader][8] is to be instantiated by setting the DecodeType.QR. The following is the sample code that reads a Swiss QR Code and displays the detail using C#.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageComplexBarcodes-ReadComplexBarcodes-ReadComplexBarcodes.cs" >}}

For more details, please visit [here][9].

## Read Information from Columbia ID Cards and Driving License

For testing purposes, we tried our product on a few used Columbia Id cards and driving licenses. It was a success and all the information was read successfully however few enhancements were done to read the information without any error. As we know that Pdf417 is used in this case which is a stacked linear barcode format used in a variety of applications such as transport, identification cards, and inventory management. "PDF" stands for Portable Data File. The "417" signifies that each pattern in the code consists of 4 bars and spaces in a pattern that is 17 units (modules) long. We have made the following enhancements in this case:

*   Enhance restoration methods for blurred Pdf417 barcodes
*   Improve basic recognition quality
*   Avoid failures during image to text conversion
*   Investigation for a multithreaded framework for Zebra target detection

## Enhancement to Read the whole Length of Barcode

There was an issue while reading the whole length of the barcode as the whole text was not read and the partial text was returned by the API. A detailed investigation was done and observed that current wiped bar restoration works only for NBase and needs changes that could be implemented for WBase based barcodes. Another problem is the absence of checksum in Code39 barcodes, which doesn’t allow to check if the result correct. All these issues were resolved and this issue was sorted out by enabling the wiped bars option.

The following sample code reads the whole length of the barcode.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageAndOptimizeBarcodeRecognition-SingleWipedBarsInPattern-SingleWipedBarsInPattern.cs" >}}

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][10]
*   [Download Aspose.BarCode for .NET][11]
*   [Aspose.BarCode for .NET Wiki docs][12] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][13] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][14] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][15] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/barcode/net/new-releases/aspose.barcode-for-.net-19.10-(dlls-only
[2]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+19.10+Release+Notes
[3]: https://apireference.aspose.com/net/barcode/aspose.barcode.complexbarcode/swissqrbill
[4]: https://apireference.aspose.com/net/barcode/aspose.barcode.complexbarcode/swissqrcodetext
[5]: https://apireference.aspose.com/net/barcode/aspose.barcode.complexbarcode/complexbarcodegenerator
[6]: https://apireference.aspose.com/net/barcode/aspose.barcode.complexbarcode/swissqrcodetext
[7]: https://docs.aspose.com/
[8]: https://apireference.aspose.com/net/barcode/aspose.barcode.complexbarcode/complexcodetextreader
[9]: https://docs.aspose.com/
[10]: https://products.aspose.com/barcode/net
[11]: https://www.nuget.org/packages/Aspose.BarCode/
[12]: https://docs.aspose.com/display/barcodenet/Home
[13]: https://forum.aspose.com/c/barcode
[14]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[15]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




