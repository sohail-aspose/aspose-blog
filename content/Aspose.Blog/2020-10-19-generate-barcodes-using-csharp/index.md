---
title: 'Generate Barcodes using C# - .NET Barcode API'
seoTitle: "C# Generate Barcodes | Generate QR Code, Code128, Aztech, Datamatrix"
description: "Generate barcode using C# or VB.NET. Generate Code128, Code11, Code39, QR, Datamatrix, EAN13, EAN8, ITF14, PDF417 and other popular barcodes using C#."
date: Mon, 19 Oct 2020 23:42:00 +0000
draft: false
url: /2020/10/19/generate-barcodes-using-csharp/
author: Usman Aziz
summary: ''
tags: ['generate barcodes using csharp', 'generate code128 barcode using csharp', 'generate qr code using csharp']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/genertae-barcodes-using-csharp.png" alt="generate barcode using C#">}}


Barcodes are used to visually represent the data in a machine-readable form. Most often, barcodes appear to be a means of a product's identification. Various types of barcodes are used in different scenarios such as Code128, QR, Datamatrix, Aztec, etc. In this article, you will learn **how to generate the barcodes in C#**. Furthermore, you will see how to customize the appearance of a barcode.

*   [C# Barcode Generator API][1]
*   [How to Generate a Barcode using C#][2]
*   [How to Generate QR Barcode using C#][3]
*   [Customize the Appearance of a Barcode in C#][4]
*   [Add Caption in Barcode using C#][5]

## C# Barcode API - Free Download {#CSharp-Barcode-Generator-API}

[Aspose.BarCode for .NET][6] is a powerful barcode generator and scanner API. It lets you generate and read a wide range of barcode symbologies, including but not limited to:

*   Code128
*   Code11
*   Code39
*   QR
*   Datamatrix
*   EAN13
*   EAN8
*   ITF14
*   PDF417
*   and [more][7].

You can [download][8] the API for free or get it installed within your .NET application using [NuGet][9].

```
PM> Install-Package Aspose.BarCode
```

## How to Generate a Barcode using C# {#Generate-Barcode-using-CSharp}

The following are the steps to generate a barcode using Aspose.BarCode for .NET.

*   First, create an object of [BarcodeGenerator][10] class and specify the barcode's type and text in its constructor.
*   Set barcode's features such as resolution and etc.
*   Finally, generate barcode using [BarcodeGenerator.Save(String)][11] method.

The following code sample shows how to generate a barcode using C#.

{{< gist aspose-com-gists 4bd7bbacc9151bf03da3125ec4559746 "generate-barcode.cs" >}}



{{< figure align=center src="images/generate-barcode-java.png" alt="generate barcode in C#">}}


## How to Generate a QR Barcode using C# {#Generate-QR-Barcode-using-CSharp}

You can generate other types of barcodes in a similar way. For the demonstration, let's generate a QR barcode. The following are the steps to generate a QR barcode.

*   Create an object of [BarcodeGenerator][12] class and specify the barcode's type as _EncodeTypes.QR_.
*   Generate barcode using [BarcodeGenerator.Save(String)][13] method.

The following code sample shows how to generate a QR barcode using C#.

{{< gist aspose-com-gists 4bd7bbacc9151bf03da3125ec4559746 "generate-QR-barcode.cs" >}}



{{< figure align=center src="images/generate-qr-barcode-java.png" alt="generate QR barcode in C#">}}


## Customize the Appearance of a Barcode in C# {#Customize-the-Appearance-of-a-Barcode-in-CSharp}

You can also customize the appearance of the barcode. For example, you can change its font, forecolor, background color, text color, and etc. The following are the steps to customize a barcode using Aspose.BarCode for .NET.

*   First, create an instance of [BarcodeGenerator][14] class.
*   Set the barcode's appearance using [BarcodeGenerator.Parameters][15] properties i.e. _BarcodeGenerator.Parameters.BackColor_.
*   Finally, generate barcode using [BarcodeGenerator.Save(String)][16] method.

The following code sample shows how to generate a customized Aztec barcode using C#.

{{< gist aspose-com-gists 4bd7bbacc9151bf03da3125ec4559746 "generate-customized-barcode.cs" >}}



{{< figure align=center src="images/generate-barcode-custom-appearance.png" alt="generate Aztec barcode in C#">}}


## Add Caption in Barcodes using C# {#Add-Caption-in-Barcode-using-CSharp}

You might have seen barcodes with a caption above or below the barcode image. These captions can be used to display additional information about the barcode itself. Aspose.BarCode for .NET also allows you to add a caption below, above, or on both sides of the barcode. The following are the steps to add a caption.

*   First, create an object of [BarcodeGenerator][17] class.
*   Set the barcode's text and type in the constructor of _BarcodeGenerator_.
*   Set caption using [CaptionAbove][18] or [CaptionBelow][19] properties.
*   Finally, save the barcode using [BarcodeGenerator.Save(String)][20] method.

The following code sample shows how to add caption in a barcode using C#.

{{< gist aspose-com-gists 4bd7bbacc9151bf03da3125ec4559746 "generate-barcode-with-caption.cs" >}}



{{< figure align=center src="images/generate-barcode-with-caption-java.png" alt="generate barcode with caption in C#">}}


## Conclusion

In this article, you have learned how to generate barcodes programmatically using C#. In addition, you have seen how to customize a barcode by modifying its appearance. You can explore more about the C# barcode generator API using [documentation][21].

## See Also

*   [Read Barcodes using C# Barcode API][22]




[1]: #CSharp-Barcode-Generator-API
[2]: #Generate-Barcode-using-CSharp
[3]: #Generate-QR-Barcode-using-CSharp
[4]: #Customize-the-Appearance-of-a-Barcode-in-CSharp
[5]: #Add-Caption-in-Barcode-using-CSharp
[6]: https://products.aspose.com/barcode/net
[7]: https://docs.aspose.com/barcode/net/barcode-supported-symbologies/
[8]: https://downloads.aspose.com/barcode/net
[9]: http://nuget.org/packages/Aspose.Barcode
[10]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[11]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/1
[12]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[13]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/1
[14]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/basegenerationparameters
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/1
[17]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[18]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/basegenerationparameters/properties/captionabove
[19]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/basegenerationparameters/properties/captionbelow
[20]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/1
[21]: https://docs.aspose.com/barcode/net/getting-started/
[22]: https://blog.aspose.com/2020/10/20/scan-and-read-barcodes-using-csharp/





