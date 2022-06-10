---
title: 'Enhancements made to the BarCodeReader with Aspose.Barcode for .NET 18.10'
date: Mon, 15 Oct 2018 07:45:16 +0000
draft: false
url: /2018/10/15/enhancements-made-to-the-barcodereader-with-aspose.barcode-for-.net-18.10/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://products.aspose.com/barcode/net)We are pleased to announce the release of [Aspose.Barcode for .NET 18.10][2]. This micro release addresses the instance reusability issue of the BarCodeReader. For a detailed note on what is new and fixed, please visit the [release notes][3] page for information of API documentation.

## Enhancements made to the BarCodeReader

Before this release, if you wanted to scan two Barcodes, you had to create a new instance of the BarCodeReader to scan the second Barcode. This release of Aspose.Barcode for .NET addresses that issue. Now you can scan multiple Barcodes using the same instance of the BarCodeReader. This is demonstrated using a simple example given below.

```
BarCodeReader barCodeReader = new BarCodeReader();
barCodeReader.SetBarCodeImage(new Bitmap("BarCode1.bmp"));
barCodeReader.SetBarCodeReadType(DecodeType.AllSupportedTypes);
while (barCodeReader.Read())
{
    Console.WriteLine("BarCode Type: " + barCodeReader.GetCodeType());
    Console.WriteLine("BarCode CodeText: " + barCodeReader.GetCodeText());
}

barCodeReader.SetBarCodeImage(new Bitmap("BarCode2.bmp"));
while (barCodeReader.Read())
{
    Console.WriteLine("BarCode Type: " + barCodeReader.GetCodeType());
    Console.WriteLine("BarCode CodeText: " + barCodeReader.GetCodeText());
}
barCodeReader.Close();
```

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   [Aspose.BarCode for .NET Wiki docs][6]– Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7]– Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8]– You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9]– We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png
[2]: https://www.nuget.org/packages/Aspose.BarCode/18.10.0
[3]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+18.10+Release+Notes
[4]: https://products.aspose.com/barcode/net
[5]: https://www.nuget.org/packages/Aspose.BarCode/
[6]: https://docs.aspose.com/display/barcodenet/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




