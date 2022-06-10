---
title: 'Support of Recognition Modes, Unicode Text Detection, Micro PDF417 and Micro QR using C#'
date: Sun, 03 May 2015 17:41:33 +0000
draft: false
url: /2015/05/03/multiple-barcode-recognition-modes-and-unicode-text-detection/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for .NET][1] 6.9.0. This new release adds support of various recognition modes and allows developers to configure unicode text detection settings. The recognition modes cater the most common failure scenarios in regard of quality, extra quality, performance and maintain balance between the speed and quality. It also controls color fill mechanism in bars of 1D barcodes, users can keep bar's color as unfilled and only maintain its borders to track a bar. This major release has new features and also enhanced old ones which you already know and love. In addition to that we keep continuity on fixing bugs and add new capabilities all the time.

## Recognition Modes Tune the Speed and Quality

The speed and quality are two important factors always influence each other. Our product team has provided new APIs to further customize the quantity of quality and performance. Since, we have provided more control to the client's end. Clients can now configure options of recognition accuracy and speed manually.  For more information, please visit Switch Barcode Recognition Modes According to the Requirement.

## Encoding of Micro PDF417 Code

Micro PDF147 code is the extended form of PDF417 code. It allows clients to encode more bytes than PDF147. Micro-PDF417 is designed for applications requiring improved area efficiency. Previously, we supported its decoding and now users can also encode Micro PDF147 codes.

## Decoding of Micro QR Code

Micro QR code is a smaller version of the QR code standard for applications where symbol size is limited. We have added its decoding support and have plans to include its encoding support in future releases.

## New Library for .NET Framework 3.5 Client Profile

In this new release, we have added a new version of library compiled under .NET Framework 3.5 Client Profile. Clients can use it for .NET Framework 3.5 Client Profile or higher.

## Detect Barcode Unicode Text

We have added the detect encoding flag, once it is enabled, the barcode engine tries to detect the encoding of the barcode and returns Unicode text. Otherwise, it returns plain text without encoding detection. Following help topic shows, how clients can detect unicode characters: Detect the Unicode Encoding of the Barcode

## Control Bars Color Filling - For 1D Barcodes Only

We have added a new FilledBars property in BarCodeBuilder class. It allows clients to generate filled or not filled bars. This property works only with 1D barcodes. Following help topic shows, how clients can not fill bars color: Control Bars Filling of the 1D Barcodes

The major areas include encoding and decoding enhancements, incorrect reading fixes of various code symbologies, enhancing of the barcode image,  improve accuracy of recognition, extra letters in codetext and improve recognition performance. This release comprises a number of key fixes that help us reading and writing capabilities.

*   Fixed: QR/Micro QR - encode/decode improvements.
*   Fixed: Code39 barcode could not be recognized from a scanned image.
*   Fixed: Can't recognize DataMatrix code from png image.
*   Fixed: Can't recognize Code128 and DataMatrix codes in a single way.
*   Fixed: Can't recognize all DataMatrix codes from a tif file.
*   Fixed: Can't recognize QR code from jpg image.
*   Fixed: Incorrect recognition of the QR code from PNG image.
*   Fixed: Can't create Code128 barcode with standard 'f' character.
*   Fixed: Can't recognize QR code from the TIF image.
*   Fixed: Can't recognize all QR codes from the JPG image.
*   Fixed: Recognizing two Code128 codes instead of one.
*   Fixed: Add support of GS1 Databar coupon code generation.
*   Fixed: Spell mistake in the XML of Aspose.BarCode API.
*   Fixed: Incorrect recognition of Pdf417 code from the tif image.
*   Fixed: Can't recognize QR code without Orientation Hints settings.
*   Fixed: Can't recognize DataMatrix code from the TIF file.
*   Fixed: Incorrect recognition of Code128 code from the tif image.
*   Fixed: Can't recognize a QR code from the PDF document.
*   Fixed: Optimize the speed of recognition from the multipage tiff file format.
*   Fixed: Incorrect encoding punctuation in PDF417 and MicroPDF417 barcodes.
*   Fixed: Incorrect recognition of Code128 code from the tif image.
*   Fixed: Can't recognize Ean13 code from the JPG image.
*   Fixed: Can't recognize Code39 code from the PDF document.
*   Fixed: Can't recognize PDF417 code from the PDF document.
*   Fixed: Can't recognize QR codes using an error correction level.
*   Fixed: Сode128 recognizer confuses f and "FNC1".
*   Fixed: Can't recognize QR code from a JPG file.
*   Fixed: Fake recognition of MicroPdf417.
*   Fixed: Extra letters in codetext when checksum off.

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][2]
*   [Download Aspose.BarCode for .NET][3]
*   [Aspose.BarCode Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://products.aspose.com/barcode
[3]: https://downloads.aspose.com/barcode
[4]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposebarcode/Aspose_BarCode_NET




