---
title: 'Micro PDF417 and Micro QR Barcode Encodings in SQL Server Reporting Services'
date: Mon, 29 Jun 2015 01:16:01 +0000
draft: false
url: /2015/06/29/micro-pdf417-micro-qr-barcode-encodings-sql-server-reporting-services/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-SSRS-e1377591419756.png" alt="Aspose.BarCode for SSRS icon">}}


Today, we’re excited to announce the new release version of [Aspose.BarCode for SSRS][1] APIs 7.0.0. This new release version covers some new barcode symbologies, full support of Microsoft SQL Server 2014, enhance its support in the Business Intelligence for Visual Studio 2013 report building and allows clients to encode barcode with empty bars. Along with these features support, we have included many other recent fixes reported by our clients in the Aspose site forums. We always appreciate our client's precious feedback.

## Encoding of QR and Micro QR Codes

For the smallest possible code users might want to consider a micro QR code because the Micro QR code is a smaller version of the QR code standard for applications where symbol size is constrained. We have added its encoding support. Many other improvements are added to QR encoding. Users can now encode QR codes in ECI mode. It also encodes a multi-ECI and FNC1 symbols. Following help topics show, how many ways users can encode QR or Micro QR codes: QR or Micro QR Barcode Encoding Selector, Generate QR Code in the ECI Mode and Generate QR Code with multi-ECI and FNC1 Symbols.

## Full Support for Microsoft SQL Server 2014

We have added full support of Microsoft SQL Server 2014. Users can now develop their reports. For Microsoft SQL Server 2014, we have provided two separate assemblies. First "Design Version" works only with designers (Visual Studio or BIDS). This assembly is located in the Bin\\SSRS2014\\DesignVersion directory. Second "RunTimeVersion" works only with the report server. This assembly is located in the Bin\\SSRS2014\\RunTimeVersion directory.

## Improvements using Business Intelligence for Visual Studio 2013

We noticed some queries from our clients in using Aspose.BarCode APIs with Business Intelligence for Visual Studio 2013. Since, we checked its support and have fixed some issues. Toolbox in Visual Studio 2013 can't detect any report component. We have already addressed this issue for Visual Studio 2012. It's now documented in our docs. Please see at step 5: Visual Studio Configuration for Aspose.BarCode APIs.

## Control Bars Color Filling – For 1D Barcodes Only

We have added a new FilledBars property in BarCodeBuilder class. It allows clients to generate filled or not filled bars. This property works only with 1D barcodes. Following help topic shows, how clients can't fill bars color: How to Display BarCode with Empty Bars.

We have enhanced OneCode and SwissPostParcel encoding areas. Already, clients had the capacity encode off base content in OneCode symbology but now it displays a proper error message. Similarly, in case of SwissPostParcel code, Aspose.BarCode APIs were adding “98″ text at the start whereas parcels always start with “99.42″. We have fixed it.

This release also comprise a number of other key fixes that help us in writing capabilities.

*   Fixed: Can't create Code128 barcode with standard 'f' character.
*   Fixed: Incorrect encoding punctuation in PDF417 and MicroPDF417 barcodes.
*   Fixed: Index out of range error message while generating a Code128 symbology.
*   Fixed: XDimension property is not working as expected.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new Symbology.MicroPdf417 and Symbology.MicroQR values have been added. It can be used to encode Micro PDF417 and Micro QR codes.
*   A new FilledBars property is added in BarCodeBuilder class. It allows clients to generate filled or not filled bars.
*   The new QREncodeType property in the BarCodeBuilder Class and QREncodeType Enum are added. This new property works as QR / MicroQR selector.
*   The new modes have been added to QREncodeMode Enum.
*   The new ECIEncoding property in the BarCodeBuilder Class and ECIEncodings Enum are added. This new property is used to tell the barcode reader details about the used references for encoding the data in the symbol by the Extended Channel Interpretation Identifiers.
*   The new QrExtCodetextBuilder class is added. It helps to generate extended code text.

## Aspose.BarCode for SSRS Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for SSRS APIs][2]
*   [Download Aspose.BarCode for SSRS][3]
*   Aspose.BarCode for SSRS Wiki docs - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://products.aspose.com/barcode/reporting-services
[2]: https://products.aspose.com/barcode/reporting-services
[3]: https://downloads.aspose.com/barcode/reporting-services
[4]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[5]: https://blog.aspose.com/




