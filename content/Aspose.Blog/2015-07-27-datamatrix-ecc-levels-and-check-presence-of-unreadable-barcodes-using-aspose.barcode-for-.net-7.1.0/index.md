---
title: 'Set DataMatrix ECC Levels and Check Presence of Unreadable Barcodes using C#'
date: Mon, 27 Jul 2015 19:24:55 +0000
draft: false
url: /2015/07/27/datamatrix-ecc-levels-and-check-presence-of-unreadable-barcodes-using-aspose.barcode-for-.net-7.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We're pleased to announce the new release version 7.1.0 of the [Aspose.BarCode for .NET APIs][1]. This new release version allows developers to select ECC levels while encoding DataMatrix code and also have added a flag to indicate the presence of not properly readable barcodes on the picture. For now, this flag is supported by QR and Code128 recognition engines and enabled by the modes: RecognitionMode.MaxBarCodes and RecognitionMode.ManualHints with ManualHint.IncorrectBarcodes. All the recognition modes have already been defined in this help topic: [Switch Barcode Recognition Modes According to the Requirement][2]. Many other important issues of reading and writing barcodes and get correct regions of the available barcode in the picture have been included.

## Select ECC Level While Encoding DataMatrix Code

Aspose.BarCode APIs allow selecting an appropriate ECC level while encoding DataMatrix barcode. The DataMatrix symbology adopts two types of error correction algorithms, depending on the ECC level employed. The ECC levels 000 to 140, which offer five different error correction levels. However, the commonly used ECC 200 level uses Reed-Solomon error correction. Following help topic shows, how to encode DataMatrix code along with the ECC algorithm: [Select an ECC Type to Encode a Barcode][3]

## Check Presence of the Unreadable Barcode

Aspose.BarCode APIs allow developers to detect whether the image contains any unreadable barcode on the picture. Following help topic shows, how to check presence of unreadable barcode on the picture: [Detect an Unreadable Barcode on the Image][4]

Many reported bug fixes have also been included. This release comprises a number of key fixes that help us reading and writing capabilities.

*   Fixed: The duplicate recognition of the DataMatrix.
*   Fixed: Incorrect recognition when lines restoration is used.
*   Fixed: Incorrect barcode read type for SwissPostParcel filter.
*   Fixed: Incorrect recognition of Planet code from the tif image.
*   Fixed: Can't recognize Aztec code from the PDF document.
*   Fixed: Can't recognize DataMatrix code from the JPG / PNG images.
*   Fixed: Can't recognize Code39 barcodes from the PDF / tif documents.
*   Fixed: SSCC18 symbology, check digit should be in parenthesis.
*   Fixed: Error message when tried to encode Code128 with FNC 3 character.
*   Fixed: Incorrect Or Unable to recognize barcodes from a PDF file format.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new GetIsDeniable method has been added to the BarCodeReader class in order to indicate whether the image contains an unreadable barcode.
*   The new DatamatrixECC property is added to the BarCodeBuilder class in order to select an appropriate ECC level while encoding DataMatrix barcode.
*   The new DataMatrixEccType Enum has been added to specify the type of the ECC to encode.

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][5]
*   [Download Aspose.BarCode for .NET][6]
*   Aspose.BarCode for .NET Wiki docs - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode
[2]: https://docs.aspose.com/display/barcodenet/Read+Barcode+Properties
[3]: https://docs.aspose.com/display/barcodenet/Use+Checksum+and+Supplement+Data#UseChecksumandSupplementData-SelectanECCTypetoEncodeaBarcode
[4]: https://docs.aspose.com/display/barcodenet/Read+Barcode+Properties#ReadBarcodeProperties-DetectanUnreadableBarcodeontheImage
[5]: https://products.aspose.com/barcode
[6]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[7]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[8]: https://blog.aspose.com/
[9]: https://github.com/asposebarcode/Aspose_BarCode_NET




