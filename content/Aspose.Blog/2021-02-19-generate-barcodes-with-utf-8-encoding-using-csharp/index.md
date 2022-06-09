---
title: 'Generate Barcodes with UTF-8 Encoding using C#'
seoTitle: "Generate Barcodes with UTF-8 Encoding using C# | Read UTF-8 Barcodes"
description: "Use .NET barcode API to generate and read barcodes using UTF-8 encoding in C#. Generate barcodes of popular symbologies with various encodings."
date: Fri, 19 Feb 2021 02:04:00 +0000
draft: false
url: /2021/02/19/generate-barcodes-with-utf-8-encoding-using-csharp/
author: Usman Aziz
summary: 'In the [previous post][1], you have seen how to generate and read different types of barcodes using C#. However, in certain cases, you have to deal with non-English characters. For example, when you work with Arabic, Latin, Greek, or similar languages. In such cases, you may need to encode the characters into Unicode standards i.e. [UTF-8][2]. In accordance with that, this article covers **how to generate and recognize barcodes using UTF-8 encoding in C#**.'
tags: ['Csharp barcode api', 'Generate Barcode with UTF-8 Encoding in Csharp', 'Read Barcode with UTF-8 Encoding in Csharp']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/scan-and-read-barcodes-using-csharp.png" alt="C# Generate Barcodes with UTF-8 Encoding">}}


In the [previous post][3], you have seen how to generate and read different types of barcodes using C#. However, in certain cases, you have to deal with non-English characters. For example, when you work with Arabic, Latin, Greek, or similar languages. In such cases, you may need to encode the characters into Unicode standards i.e. [UTF-8][4]. In accordance with that, this article covers **how to generate and read barcodes using UTF-8 encoding in C#**.

*   [C# API to Generate Barcodes using UTF-8 Encoding][5]
*   [Generate Barcode with UTF-8 Encoding in C#][6]
*   [Read Barcode with UTF-8 Encoding in C#][7]
*   [Get a Free API License][8]

## C# API to Generate Barcodes using UTF-8 Encoding {#API-to-Generate-Barcodes-using-UTF-8-Encoding}

[Aspose.BarCode for .NET][9] is a powerful C# API for barcode generation and recognition. Using the API, you can work with a wide range of barcode symbologies. In addition, the API supports generating barcodes using UTF-8 encoding. You can either [download][10] the API or install it using [NuGet][11].

```
PM> Install-Package Aspose.BarCode
```

## Generate Barcode using UTF-8 Encoding in C# {#Generate-Barcode-with-UTF-8-Encoding-in-csharp}

The following are the steps to generate barcode using UTF-8 encoding.

*   First, create an instance of [BarcodeGenerator][12] class and specify the barcode type using [EncodeTypes][13].
*   Set barcode's text using [BarcodeGenerator.CodeText][14] property.
*   Set UTF-8 text encoding using [BarcodeGenerator.Parameters.Barcode.QR.CodeTextEncoding][15] property (replace QR according to the barcode type you have specified in _BarcodeGenerator_ constructor).
*   Generate barcode using [BarcodeGenerator.GenerateBarCodeImage()][16] method and save returned image into a [Bitmap][17] object.
*   Finally, save the barcode image as a file using [Bitmap.Save(String)][18] method.

The following code sample shows how to generate a barcode using UTF-8 encoding in C#.

{{< gist aspose-com-gists 74edf30d4886c1c1afb0d7f4da68adc1 "generate-barcode-UTF8.cs" >}}

## Read UTF-8 Encoded Barcode using C# {#Recognize-Barcode-with-UTF-8-Encoding-in-csharp}

The following are the steps to recognize UTF-8 encoded barcode using C#.

*   Use [BarCodeReader][19] class to load the barcode image.
*   Loop through each [BarCodeResult][20] returned by [BarCodeReader.ReadBarCodes()][21] method.
*   Create an object of the [Encoding][22] class and set encoding to UTF-8.
*   Get the char array from the bytes returned by the [BarCodeResult][23] object.
*   Build Unicode string from the characters to get the barcode text.
*   Finally, print the retrieved barcode text.

The following code sample shows how to recognize barcodes using UTF-8 encoding in C#.

{{< gist aspose-com-gists 74edf30d4886c1c1afb0d7f4da68adc1 "read-barcode-UTF8.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you are interested in trying and using the API, you can [get a free temporary license][24].

## Conclusion

In this article, you have learned how to generate barcodes using UTF-8 encoding in C#. Furthermore, you have seen how to recognize and read a UTF-8 encoded barcode. You can explore more about the C# barcode API using the [documentation][25].

## Related Links

*   [Generate Barcodes using C#][26]
*   [Read Barcodes using C# Barcode API][27]




[1]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/
[2]: https://en.wikipedia.org/wiki/UTF-8
[3]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/
[4]: https://en.wikipedia.org/wiki/UTF-8
[5]: #API-to-Generate-Barcodes-using-UTF-8-Encoding
[6]: #Generate-Barcode-with-UTF-8-Encoding-in-csharp
[7]: #Recognize-Barcode-with-UTF-8-Encoding-in-csharp
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.com/barcode/net
[10]: https://products.aspose.com/barcode/java
[11]: https://www.nuget.org/packages/Aspose.Barcode
[12]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[13]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[14]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator/properties/codetext
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/qrparameters/properties/codetextencoding
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator/methods/generatebarcodeimage
[17]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.bitmap?view=dotnet-plat-ext-5.0
[18]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.image.save?view=dotnet-plat-ext-5.0#System_Drawing_Image_Save_System_String_
[19]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[20]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[21]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[22]: https://docs.microsoft.com/en-us/dotnet/api/system.text.encoding
[23]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/barcode/net/developer-guide/
[26]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/
[27]: https://blog.aspose.com/2020/10/20/scan-and-read-barcodes-using-csharp/





