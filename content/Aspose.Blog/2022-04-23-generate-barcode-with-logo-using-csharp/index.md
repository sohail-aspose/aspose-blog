---
title: 'Generate Barcode with Logo using C#'
date: Sat, 23 Apr 2022 11:44:28 +0000
draft: false
url: /2022/04/23/generate-barcode-with-logo-using-csharp/
author: 'Muzammil Khan'
summary: 'As a C# developer, you can easily generate barcodes with company logos or images programmatically in .NET applications. In this article, you will learn **how to generate a barcode with a logo using C#**.'
tags: ['Barcode with Image C#', 'Barcode with Logo C#', 'Generate Barcode in C#', 'QR Code in C#', 'QR Code with Image C#', 'QR Code with Logo C#']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/generate-barcode-with-logo-using-csharp.jpg" alt="Generate Barcode with Logo using C#.">}}


We commonly use barcodes to represent encoded data or information about a product or a company in a machine-readable form. Normally, we use barcodes with text labels. However, we can also generate barcodes with company logos or images programmatically in .NET applications. In this article, we will learn **how to generate a barcode with a logo using C#**.

The article shall cover the following topics:

*   [C# API to Generate Barcode with Logo][1]
*   [Generate Barcode with Logo in C#][2]
*   [Generate QR Code with Logo using C#][3]

## C# API to Generate Barcode with Logo {#CSharp-API-to-Generate-Barcode-with-Logo}

For generating barcodes with logos or images, we will be using the **_[Aspose.BarCode for .NET][4]_** API. It allows us to generate and recognize a wide range of 1D & 2D [barcode types][5]. Please either [download][6] the DLL of the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.BarCode
```

## Generate Barcode with Logo in C# {#Generate-Barcode-with-Logo-in-CSharp}

We can generate a barcode with a logo or an image by following the steps given below:

1.  Firstly, create an instance of the **_[BarcodeGenerator][8]_** class with the _**[EncodeType][9]**_ and text to encode as arguments.
2.  Optionally, set the barcode size value in pixels.
3.  Next, generate a Barcode image using the **_[GenerateBarCodeImage()][10]_** method and store it in a Bitmap.
4.  Then, load the logo image as Bitmap.
5.  After that, create a new empty Bitmap image with the height of the logo and the generated barcode image.
6.  Next, initialize the Graphics class object using the **_FromImage()_** method. It takes an empty bitmap object as an argument.
7.  Then, clear the canvas using the **_Clear()_** method.
8.  Now, call the **_DrawImage()_** method to draw the barcode image on the canvas.
9.  After that, call the **_DrawImage()_** method again to draw the logo image on the canvas.
10.  Finally, save the output using the **Image._Save()_** method. It takes the output file path as an argument.

The following code example demonstrates **how to generate a barcode with a logo image using C#**.

{{< gist aspose-com-gists 691bd86adfc648bde8c2c31f280594fc "GenerateBarcodewithLogo_CSharp_Barcode.cs" >}}



{{< figure align=center src="images/output-1.png" alt="" caption="Generate Barcode with Logo in C#">}}


## Generate QR Code with Logo using C# {#Generate-QR-Code-with-Logo-using-CSharp}

Similarly, we can also generate a QR code with a logo or an image by following the steps mentioned earlier. However, we need to set the _**[EncodeType][11]**_ as QR in the first step.

The following code example demonstrates **how to generate a QR code with a logo image using C#**.

{{< gist aspose-com-gists 691bd86adfc648bde8c2c31f280594fc "GenerateBarcodewithLogo_CSharp_QRCode.cs" >}}



{{< figure align=center src="images/QR_output-1.png" alt="" caption="Generate QR Code with Logo using C#">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][12] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to generate a barcode with a logo image**. We have also seen **how to generate a QR code with an image** programmatically. Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][13]. In case of any ambiguity, please feel free to contact us on the [forum][14].

## See Also

*   [Generate and Read Royal Mail Mailmark 2D Barcode using C#][15]
*   [Generate Barcodes using C# – .NET Barcode API][16]




[1]: #CSharp-API-to-Generate-Barcode-with-Logo
[2]: #Generate-Barcode-with-Logo-in-CSharp
[3]: #Generate-QR-Code-with-Logo-using-CSharp
[4]: https://products.aspose.com/barcode/net/
[5]: https://docs.aspose.com/barcode/net/barcode-supported-symbologies/
[6]: https://downloads.aspose.com/barcode/net
[7]: https://www.nuget.org/packages/aspose.barcode
[8]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[9]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[10]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator/methods/generatebarcodeimage
[11]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/barcode/net/
[14]: https://forum.aspose.com/c/barcode/13
[15]: https://blog.aspose.com/2022/03/03/generate-and-read-royal-mail-mailmark-2d-barcode-using-csharp/
[16]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/




