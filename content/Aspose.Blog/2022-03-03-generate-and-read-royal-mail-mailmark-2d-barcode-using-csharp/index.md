---
title: 'Generate and Read Royal Mail Mailmark 2D Barcode using C#'
date: Thu, 03 Mar 2022 16:51:19 +0000
draft: false
url: /2022/03/03/generate-and-read-royal-mail-mailmark-2d-barcode-using-csharp/
author: ''Muzammil Khan''
summary: "The Royal Mail Mailmark 2D barcode is a machine-readable barcode used in letters. It provides information about mail tracking & delivery status, delivery schedule and reporting statistics. In this article, you will learn **how to generate and read Royal Mail Mailmark 2D barcodes using C#**."
tags: ['Decode Mailmark 2D Barcode in C#', 'Generate Barcodes', 'Mailmark 2D Barcode in C#', 'Read Barcodes in C#', 'Royal Mail Barcode in C#']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/Generate-and-read-mailmark-2d-barcode-copy.jpg" alt="Generate and Read Royal Mail Mailmark 2D Barcode using C#">}}


The Royal Mail Mailmark 2D barcode is a machine-readable Complex Mail Data Mark (CMDM) barcode used in letters. It provides information about mail tracking and delivery status. It may also include additional information, such as the delivery schedule and reporting statistics. In this article, we will learn **how to generate and read Royal Mail Mailmark 2D barcodes using C#**.

The following topics shall be covered in this article:

*   [C# API to Generate and Read Royal Mail Mailmark 2D Barcodes][1]
*   [Generate Royal Mail Mailmark 2D Barcode][2]
*   [Read Royal Mail Mailmark 2D Barcode][3]

## C# API to Generate and Read Royal Mail Mailmark 2D Barcodes {#CSharp-API-to-Generate-and-Read-Royal-Mail-Mailmark-2D-Barcodes}

For generating and reading Royal Mail Mailmark 2D barcodes, we will be using the Aspose.BarCode for .NET API. It allows generating and recognizing a wide range of 1D & 2D [barcode types][4]. Please either [download][5] the DLL of the API or install it using [NuGet][6].

```
PM> Install-Package Aspose.BarCode
```

## Generate Royal Mail Mailmark 2D Barcode using C# {#Generate-Royal-Mail-Mailmark-2D-Barcode-using-CSharp}

There are three types of 2D Complex Mail Data Mark barcodes:

*   **Type 7**:
    *   Letters
    *   Barcode Size: 24 × 24 modules
    *   Physical Size: 12 × 12 mm
    *   Total Character Count: 51 Characters
    *   Customer Use: 6 spare spaces



{{< figure align=center src="images/Mailmark2DType7.png" alt="Mailmark2DType7">}}


*   **Type 9**:
    *   Large Letters, including poly wrap  
        letters.
    *   Barcode Size: 32 × 32 modules
    *   Physical Size: 16 × 16 mm
    *   Total Character Count: 90 Characters
    *   Customer Use: >25 but max of 45 spare spaces



{{< figure align=center src="images/Mailmark2DType9.png" alt="Mailmark2DType9">}}


*   **Type 29**:
    *   Large Letters, including poly wrap letters.
    *   Barcode Size: 16 × 48 modules
    *   Physical Size: 8 × 24 mm
    *   Total Character Count: 70 Characters
    *   Total Character Count: need 6-25 customer characters



{{< figure align=center src="images/Mailmark2DType29.png" alt="Mailmark2DType29">}}


We can generate Royal Mail Mailmark 2D barcode by following the steps given below:

1.  Firstly, create an instance of the **_[Mailmark2DCodetext][7]_** class.
2.  Next, set various properties such as _UPUCountryID_, _VersionID_, Class, _ItemID_, etc.
3.  Then, set **_[Mailmark2DType][8]_** as Type\_7, Type\_9, or Type\_29.
4.  Next, create an instance of the **_[ComplexBarcodeGenerator][9]_** class with **_Mailmark2DCodetext_** object as an argument.
5.  After that, set the barcode dimensions.
6.  Finally, call the **_[Save][10]_** method to save the barcode image on the local disk.

The following code example demonstrates **how to generate a Mailmark 2D barcode of type 7 using C#**.

{{< gist aspose-com-gists 2afb872cc645ede3454c59fbac522253 "GenerateAndReadMailmark2DBarcode_CSharp_Generate.cs" >}}

## Read Royal Mail Mailmark 2D Barcode using C# {#Read-Royal-Mail-Mailmark-2D-Barcode-using-CSharp}

We can read Royal Mail Mailmark 2D barcode by following the steps given below:

1.  Firstly, create an instance of the **_[BarCodeReader][11]_** class.
2.  Next, provide the input barcode image path and the **_[DecodeType][12]_**.
3.  Then, get the **_[BarCodeResult][13]_** by calling the **_[ReadBarCodes()][14]_** method.
4.  After that, decode the barcode using the **_[TryDecodeMailmark2D()][15]_** method.
5.  Finally, read decoded properties of the **_Mailmark2DCodetext_** object.

The following code example demonstrates **how to read a Mailmark 2D barcode using C#**.

{{< gist aspose-com-gists 2afb872cc645ede3454c59fbac522253 "GenerateAndReadMailmark2DBarcode_CSharp_Read.cs" >}}

```
UPUCountryID:JGB
InformationTypeID:0
VersionID:1
Class:1
SupplyChainID:123
ItemID:1234
DestinationPostCodeAndDPS:QWE1
RTSFlag:0
ReturnToSenderPostCode:QWE2
CustomerContent:CUSTOM DATA
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][16] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to generate Royal Mail Mailmark 2D barcodes** and save barcode images on the disk. We have also seen **how to read the generated Mailmark 2D barcodes** programmatically. Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][17]. In case of any ambiguity, please feel free to contact us on the [forum][18].

## See Also

*   [Read Barcodes using C#][19]
*   [Generate Barcodes using C# – .NET Barcode API][20]




[1]: #CSharp-API-to-Generate-and-Read-Royal-Mail-Mailmark-2D-Barcodes
[2]: #Generate-Royal-Mail-Mailmark-2D-Barcode-using-CSharp
[3]: #Read-Royal-Mail-Mailmark-2D-Barcode-using-CSharp
[4]: https://docs.aspose.com/barcode/net/barcode-supported-symbologies/
[5]: https://downloads.aspose.com/barcode/net
[6]: https://www.nuget.org/packages/aspose.barcode
[7]: https://apireference.aspose.com/barcode/net/aspose.barcode.complexbarcode/mailmark2dcodetext
[8]: https://apireference.aspose.com/barcode/net/aspose.barcode.complexbarcode/mailmark2dtype
[9]: https://apireference.aspose.com/barcode/net/aspose.barcode.complexbarcode/complexbarcodegenerator
[10]: https://apireference.aspose.com/barcode/net/aspose.barcode.complexbarcode.complexbarcodegenerator/save/methods/1
[11]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[12]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/basedecodetype
[13]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[14]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.complexbarcode/complexcodetextreader/methods/trydecodemailmark2d
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/barcode/net/
[18]: https://forum.aspose.com/c/barcode/13
[19]: https://blog.aspose.com/2020/10/20/scan-and-read-barcodes-using-csharp/
[20]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/




