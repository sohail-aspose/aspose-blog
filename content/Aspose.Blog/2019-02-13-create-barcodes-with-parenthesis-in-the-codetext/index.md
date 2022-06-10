---
title: 'Create Barcodes with parenthesis in the CodeText'
date: Wed, 13 Feb 2019 18:41:30 +0000
draft: false
url: /2019/02/13/create-barcodes-with-parenthesis-in-the-codetext/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://products.aspose.com/barcode/net)We are pleased to announce the release of [Aspose.BarCode for .NET 19.1][2]. This release enhanced the **BarCodeGenerator** API to support parenthesis in the **CodeText**. For a detailed note on what is new and fixed, please visit the [release notes][3] page for information of API documentation.

## Support for parenthesis in CodeText

This release of Aspose.BarCode enhanced the **BarCodeGenerator** API to allow the **CodeText** to contain parenthesis. You may generate barcodes with parenthesis in the **CodeText** as shown below in the code example. 

```
Aspose.BarCode.Generation.BarCodeGenerator generator = new  
Aspose.BarCode.Generation.BarCodeGenerator(  
Aspose.BarCode.Generation.EncodeTypes.Pdf417);  
  
generator.CodeText = "Sample.Code.Text(Example).20181203\_150435";  
  
generator.Save(TestDirectory + "barcodeTest.png", BarCodeImageFormat.Png);
```
```
Result:  
Correct PNG image.
```

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   [Aspose.BarCode for .NET Wiki docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png
[2]: https://www.nuget.org/packages/Aspose.BarCode/19.1.0.1
[3]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+19.1+Release+Notes
[4]: https://products.aspose.com/barcode/net
[5]: https://www.nuget.org/packages/Aspose.BarCode/
[6]: https://docs.aspose.com/display/barcodenet/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




