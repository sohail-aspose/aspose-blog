---
title: 'Recognize BarCodes using new Decode Types in Aspose.BarCode for .NET'
date: Tue, 11 Dec 2018 17:47:05 +0000
draft: false
url: /2018/12/11/recognize-barcodes-using-new-decode-types-in-aspose.barcode-for-.net-18.11/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Barcode for .NET 18.11][1]. This release added new Decode Types in the API for better recognition of Barcodes. For a detailed note on what is new and fixed, please visit the [release notes][2] page for information of API documentation.

## New subsets in DecodeType

The new release of Aspose.Barcode provides additional Decode types which enhance the performance and ease of reading barcodes. You may use the newly added Decode types as shown below.

```
using (BarCodeReader reader = new BarCodeReader("test.png", 
DecodeType.Types1D))
{
    while (reader.Read())
    {
        Console.WriteLine(reader.GetCodeType().ToString() 
        + " " + reader.GetCodeText());
    }
}

using (BarCodeReader reader = new BarCodeReader("test.png", 
DecodeType.PostalTypes))
{
    while (reader.Read())
    {
        Console.WriteLine(reader.GetCodeType().ToString() 
        + " " + reader.GetCodeText());
    }
}

using (BarCodeReader reader = new BarCodeReader("test.png",
 DecodeType.MostCommonTypes))
{
    while (reader.Read())
    {
        Console.WriteLine(reader.GetCodeType().ToString() 
        + " " + reader.GetCodeText());
    }
}
```

## Other Enhancements in API

Other than the addition of decode types, there are a number of other enhancements made to the API in this release. These enhancements are listed below:

*   Barcode reader has been enhanced with improved detection of the following barcodes
    *   3D-distorted barcodes
    *   2D-rotated barcodes
    *   CODE39 barcodes
*   WPF control appearance has been improved.
*   GS1 DataBar Expanded Stacked barcode passes the GS1 Canada barcode verification.
*   You can now constrain the region for barcode detection to improve performance.
*   Enhanced MicrE13B for safe bitmap access.

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   [Aspose.BarCode for .NET Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.BarCode/18.11.0
[2]: https://docs.aspose.com/barcode/net/aspose-barcode-for-net-18-11-release-notes/
[3]: https://products.aspose.com/barcode/net
[4]: https://www.nuget.org/packages/Aspose.BarCode/
[5]: https://docs.aspose.com/barcode/net/
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




