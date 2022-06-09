---
title: 'Read Barcodes using C# Barcode API'
seoTitle: ""
description: ""
date: Tue, 20 Oct 2020 23:42:00 +0000
draft: false
url: /2020/10/20/scan-and-read-barcodes-using-csharp/
author: Usman Aziz
summary: ''
tags: ['csharp barcode reader', 'csharp barcode scanner', 'read barcodes in csharp', 'scan barcodes in csharp']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/scan-and-read-barcodes-using-csharp.png" alt="scan and read barcode in C#">}}


In the [previous article][1], you have learned how to generate various types of barcodes programmatically. In this article, you will learn **how to read the barcodes using C# barcode reader API**. The article will also cover how to read particular or different types of barcode symbologies in an image.

*   [C# Barcode Reader API][2]
*   [Read Barcodes using C#][3]
*   [Scan and Read a Particular Barcode Symbology in C#][4]
*   [Multiple Barcode Symbologies in a Single Image][5]

## C# API to Read Barcodes {#CSharp-Barcode-Scanner-and-Reader-API}

[Aspose.BarCode for .NET][6] provides a powerful barcode scanner and reader API that lets you read a variety of barcode symbologies within a few lines of code. You can either [download][7] the API or install it within your .NET application using [NuGet][8].

```
PM> Install-Package Aspose.BarCode
```

## Read Barcodes using C# {#Scan-and-Read-Barcodes-using-CSharp}

The following are the steps to read a 1D or 2D barcode from an image file.

*   Create an object of [BarCodeReader][9] class and specify the image's file path.
*   Use [BarCodeResult][10] class to fetch the recognition results from [BarCodeReader.ReadBarCodes()][11] method.
*   Retrieve barcode's type and text from [BarCodeResult][12] object.

The following code sample shows how to read a barcode using C#.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "read-barcode.cs" >}}

## Read a Particular Barcode Symbology in C# {#can-and-Read-a-Particular-Barcode-Symbology-in-CSharp}

There could be the case when you already know about the symbology of the barcode you are going to read. In such situations, you can provide the barcode's type to the [BarCodeReader][13]'s object. Knowing the type beforehand speeds up the barcode recognition process. The following code sample shows how to specify the barcode's type.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageAndOptimizeBarcodeRecognition-RecognizeSpecificBarcodeSymbology-RecognizeSpecificBarcodeSymbology.cs" >}}

## Scan Multiple Barcode Symbologies in a Single Image {#Read-Multiple-Barcode-Symbologies-in-a-Single-Image}

In particular cases, you might have multiple barcode symbologies placed in a single image. For such a case, you can configure the API to recognize all the barcodes in one go. The following are the steps to read multiple barcodes in a single image.

*   Create an array of [BaseDecodeType][14] to contain the list of barcode symbologies.
*   Create an object of the [BarCodeReader][15] class and load the image.
*   Read barcodes using [BarCodeReader.ReadBarCodes()][16] and extract their type and text.

The following code sample shows how to read multiple barcode symbologies in a single image using C#.

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageAndOptimizeBarcodeRecognition-RecognizeMultipleSymbologies-RecognizeMultipleSymbologies.cs" >}}

## Conclusion

In this article, you have learned how to read barcodes programmatically using C#. In addition, you have seen how to read one or multiple barcode symbologies in a single image. You can learn more about C# barcode reader API using the [documentation][17].

## See Also

*   [Generate Barcodes using C# – .NET Barcode API][18]




[1]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/
[2]: #CSharp-Barcode-Scanner-and-Reader-API
[3]: #Scan-and-Read-Barcodes-using-CSharp
[4]: #can-and-Read-a-Particular-Barcode-Symbology-in-CSharp
[5]: #Read-Multiple-Barcode-Symbologies-in-a-Single-Image
[6]: https://products.aspose.com/barcode/net
[7]: https://downloads.aspose.com/barcode/net
[8]: http://nuget.org/packages/Aspose.Barcode
[9]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[10]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[11]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[12]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[13]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[14]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/basedecodetype
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[17]: https://docs.aspose.com/barcode/net/getting-started/
[18]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/





