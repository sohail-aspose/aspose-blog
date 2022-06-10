---
title: 'Generate Postal Barcode in C# with Aspose.BarCode for .NET 17.8'
date: Thu, 07 Sep 2017 18:50:05 +0000
draft: false
url: /2017/09/07/enhanced-postal-barcode-generation-with-aspose.barcode-for-.net-17.8/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="Aspose.Barcode for .NET">}}


Aspose.Barcode for .NET 17.8 has been released. The major development in this release is the enhanced functionality of Aspose.BarCode to generate postal barcode with specified height. In the previous versions, it was not possible to set the height of bars for Postal barcodes like Postnet, AustraliaPost etc. Improved GS1Code128 coded barcode recognition functionality has also been incorporated in this release.

## Enhanced Postal Barcode Generation in C#

In the old versions of Aspose.BarCode, it was not possible to set the height of bars of Postal barcodes like postnet, AustraliaPost, Planet, OneCode and RM4SCC. Aspose.Barcode for .NET 17.8 now allows developers to set the bar height. The said functionality is illustrated in the following code sample.

```
// Create an instance of BarCodeBuilder class
using (BarCodeBuilder barCodeBuilder = new BarCodeBuilder())
{
    // Set barcode text
    // Set encoding type
    barCodeBuilder.CodeText = "12345678";
    barCodeBuilder.EncodeType = EncodeTypes.Postnet;
 
    // Set barcode Dimension and height
    barCodeBuilder.xDimension = 1f;
    barCodeBuilder.BarHeight = 40;
 
    // Save the barcode image
    barCodeBuilder.Save("postnet.png");
}
```

## Other Improvements

This release also fixes exceptions that were reported by our valued customers. The complete list of enhancements and fixes in this release is as follows.

*   Process of GS1Code128 coded barcode recognition has been enhanced. The functionality has been improved in such a way that it now recognize correct type of GS1Code128 coded barcode.
*   Process of generating EAN14 barcode has been improved.
*   Functionality to recognize DatabarStacked coded barcode has been improved.
*   Functionality of yDimension property has been enhanced. It is now working for 2D barcodes e.g. CodablockF.

To view a complete list of enhancements and fixes, please visit the [release notes][1] page. You can download the latest version by visiting the [Aspose.Barcode for .NET 17.8][2] page in the downloads section.

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes, and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+17.8+Release+Notes
[2]: https://downloads.aspose.com/barcode/net
[3]: https://www.aspose.com/products/barcode/net
[4]: https://downloads.aspose.com/barcode/net
[5]: https://docs.aspose.com/display/barcodenet/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




