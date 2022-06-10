---
title: 'Generate or Read DutchKix and DotCode Barcodes using C#'
date: Tue, 28 Jun 2016 11:54:58 +0000
draft: false
url: /2016/06/28/generate-or-read-dutchkix-and-dotcode-barcodes-using-aspose.barcode-for-.net-8.0.0/
author: Muhammad Ijaz
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of Aspose.Barcode for .NET 8.0.0. This release supports [generating][1] and [reading][2] DutchKix and DotCode barcode types. Several new enhancements have also been made to barcode recognition algorithm to further improve the recognition process when reading barcodes from poor quality QR, Code128, DataMatrix and Aztec codes.

## Generate DutchKix or DotCode Barcodes using C#

Aspose.Barcode for .NET allows you to generate DutchKix or DotCode barcodes. You can set **BarCodeBuilder.SymbologyType** to **DutchKix** or **DotCode** to generate these barcodes e.g.

```
 BarCodeBuilder builder = new BarCodeBuilder(@"!AA-11;", Symbology.DotCode);
builder.Save("DotCode.png");
```

## Enhancements

Following is a list of improvements included in this release.

*   Improve algorithm to read barcodes even if the image is not rotated
*   Improve algorithm to Read the barcodes from a PNG image having 100 multiple barcodes in it
*   Improve algorithm to detect the barcodes with default settings
*   Support recognition of invasion in the quiet zone for a data matrix
*   Improve 3D-distorted Aztec code recognition
*   Improve recognition of the Aztec code
*   Recognize poor quality code128 with histogram method
*   Fix the issue with Rows property for PDF417 barcode
*   Investigate and fix order of recognizing barcodes
*   Improve DotCode regions recognition
*   Read the corrupted QR barcode

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for .NET 8.0.0 page in downloads section][3].

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   Aspose.BarCode for .NET Wiki docs – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://docs.aspose.com/
[2]: https://docs.aspose.com/display/barcodenet/Read+Barcodes
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[4]: https://products.aspose.com/barcode
[5]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[7]: https://blog.aspose.com/
[8]: https://github.com/asposebarcode/Aspose_BarCode_NET




