---
title: 'Compact PDF417 Barcode Reader and Micro QR Code Encoder in C# .NET'
date: Tue, 16 Jun 2015 16:18:11 +0000
draft: false
url: /2015/06/16/compact-pdf417-decoding-and-micro-qr-code-encoding-supports-in-aspose.barcode-for-.net-7.0.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


Today, we're excited to announce the new release version of Aspose.BarCode for .NET APIs 7.0.0. Using this new release version, users can now decode Compact PDF417 codes from the barcode picture. They can also encode Micro QR code, including ECI and FNC1 symbols. There are many ECI encoding types and users can manage it. They can even encode multiple ECI and FNC1 symbols in the QR code. Besides the above new features, we also bring performance, quality, and correct code reading improvements by fixing already reported issues.

## Read Compact PDF417 Barcode in C#

We have added support of CompactPDF417 code decoding. Compact PDF417 is referred to as Truncated PDF417 in previous standards. Compact PDF417 may be used where space is a primary concern and the symbol damage is unlikely, such as in an office environment. It removes the right row indicator and reduces the stop pattern into a single bar. Please check the list of all supported barcode symbologies: [Key Product Features][1]

## Encode QR and Micro QR Codes in C#

Micro QR code is a smaller version of the QR code standard for applications where symbol size is limited. We have added its encoding support. In the previous version, we have already added its decoding support. Many other enhancements are added to QR encoding. Users can now encode QR codes in ECI mode. It also encodes a multi-ECI and FNC1 symbols. Following help topics show, how many ways users can encode QR or Micro QR codes: [How to Create a QR or Micro QR Barcode][2], [QR Code Encoding in the ECI Mode][3], and [Encode multi-ECI and FNC1 Symbols in QR Code][4].

## Encoding of OneCode and SwissPostParcel Symbologies

In this new release version, we have improved OneCode and SwissPostParcel encoding areas. Previously, users were able to encode incorrect text in OneCode symbology but now it displays a proper error message. Similarly, in the case of SwissPostParcel code, Aspose.BarCode APIs were adding "98" text at the start whereas parcels always start with "99.42". We have fixed it.

The major areas include encoding and decoding enhancements, incorrect reading fixes of various code symbologies, enhancing of the barcode image, improve the accuracy of recognition, incorrect letters in code text, and improve recognition performance. This release comprises a number of key fixes that help us reading and writing capabilities.

*   Fixed: Can't recognize small Code128 barcodes.
*   Fixed: Detected barcode region points are incorrect.
*   Fixed: Recognize code128 with skipping bars.
*   Fixed: Can't recognize all code 128 codes from the JPG file.
*   Fixed: Can't recognize PDF417 code from the PDF and PNG files.
*   Fixed: XDimension property is not working as expected.
*   Fixed: There is no barcode but can recognize Code128 code.
*   Fixed: Incorrect recognition of Code128 from the JPEG file.
*   Fixed: Can't recognize QR barcode from the PDF and PNG files.
*   Fixed: Can't recognize all Code128 barcodes from the PDF and JPG files.
*   Fixed: Can't recognize Code128 barcode from the PDF document.
*   Fixed: Incorrect detection of DataMatrix symbology and code text of Code128 symbology.

## Public API Changes

The following API changes in the new version are also worth noting:

*   A new BarCodeReadType.CompactPdf417 value has been added. It can be used to read compact PDF417 codes.
*   The new QREncodeType property in the BarCodeBuilder Class and QREncodeType Enum are added. This new property works as a QR / MicroQR selector.
*   The new modes have been added to QREncodeMode Enum.
*   The new ECIEncoding property in the BarCodeBuilder Class and ECIEncodings Enum are added. This new property is used to tell the barcode reader details about the used references for encoding the data in the symbol by the Extended Channel Interpretation Identifiers.
*   The new QrExtCodetextBuilder class is added. It helps to generate extended code text.

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][5]
*   [Download Aspose.BarCode for .NET][6]
*   [Aspose.BarCode for .NET Wiki docs][7] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][8] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][9] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/.net/barcode-component/key-features.aspx
[2]: https://docs.aspose.com/display/barcodenet/QR+and+Micro+QR+Barcode
[3]: https://docs.aspose.com/display/barcodenet/QR+and+Micro+QR+Barcode#QRandMicroQRBarcode-QRCodeEncodingintheECIMode
[4]: https://docs.aspose.com/display/barcodenet/QR+and+Micro+QR+Barcode#QRandMicroQRBarcode-Encodemulti-ECIandFNC1SymbolsinQRCode
[5]: https://products.aspose.com/barcode
[6]: https://downloads.aspose.com/barcode
[7]: http://docs.aspose.com/display/barcodenet/Home
[8]: http://forum.aspose.com
[9]: https://blog.aspose.com/
[10]: https://github.com/asposebarcode/Aspose_BarCode_NET




