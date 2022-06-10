---
title: 'Support for silverlight barcode reader &amp; generator control and generate Aztec coded barcode using Aspose.BarCode for .NET 8.2.0'
date: Thu, 01 Sep 2016 07:29:02 +0000
draft: false
url: /2016/09/01/support-for-silverlight-barcode-reader-generator-control-and-generate-aztec-coded-barcode-using-aspose.barcode-for-.net-8.2.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png) We are pleased to announce the release of Aspose.Barcode for .NET 8.2.0. This release supports generating and reading Aztec barcode type. This release supports checksum validation for OneCode and AustraliaPost coded barcodes. Support for silverlight barcode reader & generator control and support for setting graphics unit in compact framework have also been incorporated in this release.

## Generate Aztec barcode

Aspose.Barcode for .NET allows you to generate Aztec barcode. You can set **BarCodeBuilder.SymbologyType** to **Aztec** to generate Aztec barcode e.g.

```
 BarCodeBuilder builder = new BarCodeBuilder("25", Symbology.Aztec);
builder.Save("Aztec.png"); 
```

A property **AztecSymbolMode** has been introduced to allow only numbers from 0 to 255 while using Aztec barcode. When AztecSymbolMode property is set, reader automatically detects Runes. Following is the code demonstration.

```
 // Create an instance of BarCodeBuilder class.
BarCodeBuilder b = new BarCodeBuilder();

// Set the Code text.
b.CodeText = "25";

// Set the barcode type.
b.SymbologyType = Symbology.Aztec;

// set the AztecSymbolMode property.
b.AztecSymbolMode = AztecSymbolMode.Rune;

// Save the barcode as PNG image.
b.BarCodeImage.Save("testRune25.png"); 
```

## Checksum validation for OneCode and AustraliaPost barcodes

Aspose.Barcode for .NET now supports checksum validation for OneCode and AustraliaPost barcodes. Property **ChecksumValidation** has been introduced to perform validation on OneCode and AustraliaPost barcodes. Following is the sample code demonstrating how **ChecksumValidation** can be set to off and on to perform validation.

```
 // Create an instance of BarCodeReader class and load an existing oncecode barcode.
using (BarCodeReader r = new BarCodeReader("onecode.png", DecodeType.OneCode))
{
    // Set the ChecksumValidation property to Off.
    r.ChecksumValidation = ChecksumValidation.Off;

    while (r.Read())
    {
        Console.WriteLine(r.GetCodeType() + ": " + r.GetCodeText());
        Console.WriteLine("CheckSum: " + r.GetCheckSum());
    }
} 
```

## Setting graphics unit in compact framework

Using Aspose.Barcode for .NET, developers can set the graphics unit of the bars in the barcode while they are working with compact framework. Following is the sample code snippet to set the graphics unit to millimeter in compact framework.

```
 // Create an instance of BarCodeBuilder class.
// Set the symbology and code text.
BarCodeBuilder builder = new BarCodeBuilder("12345", Symbology.Code39Standard);

// Set the GraphicsUnit property to Millimeter.
builder.GraphicsUnit = Aspose.BarCode.GraphicsUnit.Millimeter;

// Set the dimension and bar height
builder.xDimension = 0.22f;
builder.BarHeight = 15f;

// Set the barcode resolution.
builder.Resolution = new Resolution(72, 72, ResolutionMode.Customized);

// for .NET 2.0 and upper, to compare results, set margins like default of compact edition
builder.Margins = new MarginsF(8, 6, 4, 2);

System.Drawing.Bitmap barcodeImage = builder.GenerateBarCodeImage();

// compact case: put to pictureBox
pictureBox1.Image = barcodeImage;

// .NET 2.0 and upper: save to file
 barcodeImage.Save("barcode.png", System.Drawing.Imaging.ImageFormat.Png); 
```

## Enhancements

Following is a list of improvements included in this release.

*   Process of reading Postnet barcode has been improved.
*   Process of reading DataMatix barcode has been improved.
*   Functionality to set resolution in compact framework has been incorporated.
*   Processing of Dutch KIX barcodes has been improved.
*   Functionality to process the Aztec barcode with long code text has been improved.
*   Functionality to read barcode from a PDF file has been improved.
*   Functionality to read EAN13 barcode along with supplement code text has been improved.

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for .NET 8.2.0 page in downloads section][2].

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[3]: https://www.aspose.com/products/barcode/net
[4]: https://downloads.aspose.com/barcode/net
[5]: https://docs.aspose.com/display/barcodenet/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




