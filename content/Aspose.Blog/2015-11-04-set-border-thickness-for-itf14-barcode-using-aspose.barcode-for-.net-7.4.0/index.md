---
title: 'Set Border Thickness for ITF14 Barcode using Aspose.BarCode for .Net 7.4.0'
date: Wed, 04 Nov 2015 18:11:32 +0000
draft: false
url: /2015/11/04/set-border-thickness-for-itf14-barcode-using-aspose.barcode-for-.net-7.4.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png) We are pleased to announce the release of Aspose.BarCode for .NET 7.4.0. Barcode recognition from 38×18 pixel images and setting border thickness for ITF14 barcode are top of the list in this release. It also includes encoding and decoding improvements based on the clients' feedback.

## Specify Border Thickness for ITF14 Barcode

Aspose.BarCode for .Net provides facility to set border thickness for ITF14 barcode.

Following is the simple code snippet demonstrating the usage of the said property to set border thickness for ITF14 barcode.

```
 // Instantiate barcode object
BarCodeBuilder builder = new BarCodeBuilder("00850006000227");

// Set Barcode Symbology
builder.SymbologyType = Symbology.ITF14;

// Set ITF14 Barcode Border Type
builder.ITF14BorderType = ITF14BorderType.BarOut;

// Set border thickness
builder.ITF14BorderThickness = 4.83f;

// Save the Barcode image
builder.Save("ITF14 border thickness.png", BarCodeImageFormat.Png); 
```

## Enhancements

Some problems were noticed with BarHeight property of the BarCodeBuilder class and with DatabarStackedOmniDirectional barcode encoding. All such noticed areas have been improved.

*   ITF14 encoding, functionality of BarCodeBuilder.BarHeight property has been improved.
    
*   UPCA encoding, functionality of BarCodeBuilder.BarHeight property has been improved.
    
*   Recognizing DataMatrix code from the JPG image has been improved.
    
*   DataBarStackedOmniDirectional encoding, functionality of BarCodeBuilder.BarHeight property has been improved.
    
*   Setting Barcode width up to 5mil.
    
*   Recognizing Code128 and DataMatrix barcodes from jpg image has been further improved.
    

Many reported bug fixes have also been included. This release comprises a number of key fixes that help in generating barcode and barcode recognition capabilities. Please check the release notes of [Aspose.BarCode for .Net 7.4.0][2] for a complete list of enhancements.

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx "Aspose.BarCode for .NET APIs"
[3]: https://www.aspose.com/products/barcode/net
[4]: https://downloads.aspose.com/barcode/net
[5]: https://docs.aspose.com/display/barcodenet/Home
[6]: https://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




