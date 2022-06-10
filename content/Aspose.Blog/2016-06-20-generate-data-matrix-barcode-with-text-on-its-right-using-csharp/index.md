---
title: 'Generate Data Matrix Barcode with Text on its Right using C#'
date: Mon, 20 Jun 2016 08:09:17 +0000
draft: false
url: /2016/06/20/generate-data-matrix-barcode-with-text-on-its-right-using-csharp/
author: Muhammad Ijaz
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Barcode for .NET][1] 7.9.0. This release supports showing the code text on the right side of the barcode. A new algorithm has also been implemented which allows you to read 3D-distorted Aztec codes.

## Generate Data Matrix Barcode with Text on its Right

Aspose.Barcode for .NET allows you to set the code text location to the right side of the barcode. This is helpful in showing the code text on the right side of a data matrix barcode. **BarCodeBuilder.CodeLocation** can be set to **CodeLocation.Right** e.g.

```
string gtin = "898978777776665655";
string uid = "121212121212121212";
string batch = "GH768";
string expDate = "150923";

string textToEncode = gtin + uid + batch + expDate; // or  "(01)"+ gtin + "(..)"+ uid + ...
string textToDisplay = "GTIN:" + gtin + "\nUID:" + uid + "\nBatch:" + batch + "\nExp.Date:" + expDate;

BarCodeBuilder builder = new BarCodeBuilder(textToEncode, Symbology.DataMatrix);
//In order to avoid including all the names into the codetext, the property called "Display2DText" should be used.
builder.Display2DText = textToDisplay;
builder.CodeLocation = CodeLocation.Right;
builder.Margins = new MarginsF(0, 0, 0, 0);

builder.Save("codetextRightDisplay.png");
```

## Enhancements

Following is a list of improvements included in this release.

*   Aztec codes recognition has been improved 
*   Verify APTCACheck for Aspose.Barcode DLL 
*   QR barcode recognition has been improved

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for .NET 7.9.0 page in downloads section][2].

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://downloads.aspose.com/barcode
[3]: https://products.aspose.com/barcode
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[5]: https://docs.aspose.com/barcode/net
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/
[8]: https://github.com/asposebarcode/Aspose_BarCode_NET




