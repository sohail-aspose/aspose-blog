---
title: 'Generate Code128C and Aztec Barcode using Java'
date: Mon, 03 Oct 2016 20:19:06 +0000
draft: false
url: /2016/10/03/generate-code128c-and-aztec-barcode-using-java-barcode-api/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="Aspose.BarCode for Java logo">}}


We are pleased to announce the release of [Aspose.Barcode for Java][1] 8.2.0. This release supports generating and reading Aztec barcode type. This release supports checksum validation for OneCode and AustraliaPost coded barcodes. Support to apply Metered key has also been incorporated in this release.

## Generate Aztec Barcode using Java

Aspose.Barcode for Java allows you to generate Aztec barcode. You can set **BarCodeBuilder.SymbologyType** to **Aztec** to generate Aztec barcode e.g.

```
 // Initialize BarCode builder class object
BarCodeBuilder builder = new BarCodeBuilder();

// Set the barcode text
builder.setCodeText("25");

// Set symbology type as Aztec 
builder.setSymbologyType(Symbology.Aztec);

// save barcode
builder.save("Aztec.png");
```

A property **setAztecSymbolMode** has been introduced to allow only numbers from 0 to 255 while using Aztec barcode. When **setAztecSymbolMode** property is set, reader automatically detects Runes. Following is the code demonstration.

```
// Create an instance of BarCodeBuilder class.
BarCodeBuilder b = new BarCodeBuilder();

// Set the Code text.
b.setCodeText("25");

// Set the barcode type.
b.setSymbologyType(Symbology.Aztec);

// set the AztecSymbolMode property.
b.setAztecSymbolMode(AztecSymbolMode.Rune);

// Save the barcode as PNG image.
b.getBarCodeImage().save("testRune25.png");
```

## Checksum Validation for OneCode and AustraliaPost Barcodes

Aspose.Barcode for Java now supports checksum validation for OneCode and AustraliaPost barcodes. Property **setChecksumValidation** has been introduced to perform validation on OneCode and AustraliaPost barcodes. Following is the sample code demonstrating how **setChecksumValidation** can be set to off and on to perform validation.

```
// Create an instance of BarCodeReader class and load an existing oncecode barcode.
BarCodeReader r = new BarCodeReader("onecode.png", DecodeType.ONE_CODE);

// Set the ChecksumValidation property to Off.
r.setChecksumValidation(ChecksumValidation.Off);

while (r.read())
{
        System.out.println(r.getCodeType() + ": " + r.getCodeText());
        System.out.println("CheckSum: " + r.getCheckSum());
}
```

## Applying Metered Key

Aspose.Barcode for Java has introduced a new class **Metered** to apply metered key. Following is the sample code demonstrating how to set metered public and private key.

```
// Create an instance of Metered class
Metered matered = new Metered();

// Access the setMeteredKey property and pass public and private keys as parameters
matered.setMeteredKey("PublicKey", "PrivateKey");
```

## Enhancements

Following is a list of improvements included in this release.

*   Process of reading Postnet barcode has been improved.
*   Process of reading DataMatix barcode has been improved.
*   Processing of Dutch KIX barcodes has been improved.
*   Functionality to process the Aztec barcode with long code text has been improved.
*   Functionality to read barcode from a PDF file has been improved.
*   Functionality to read EAN13 barcode along with supplement code text has been improved.
*   Process of generating AustraliaPost barcode has been improved.

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for Java 8.2.0][2] page in downloads section.

## Aspose.BarCode for Java Resources

The resources you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][3]
*   [Download Aspose.BarCode for Java][4]
*   [Aspose.BarCode for Java Wiki docs][5] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/java
[2]: http://www.aspose.com/downloads/barcode/java
[3]: https://products.aspose.com/barcode
[4]: https://downloads.aspose.com/barcode/java
[5]: https://products.aspose.com/barcode/java
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




