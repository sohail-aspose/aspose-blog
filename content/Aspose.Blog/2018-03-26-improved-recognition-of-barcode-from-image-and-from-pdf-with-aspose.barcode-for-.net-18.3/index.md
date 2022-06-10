---
title: 'Improved Barcode Recognition From Image and  PDF using C#'
date: Mon, 26 Mar 2018 07:18:06 +0000
draft: false
url: /2018/03/26/improved-recognition-of-barcode-from-image-and-from-pdf-with-aspose.barcode-for-.net-18.3/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="Aspose.Barcode for .NET">}}


We are pleased to announce the release of [Aspose.BarCode for .NET][1] 18.3. This is a maintenance release whereby we have resolved some incurring issues in API.

## Improved Barcode Recognition From Image and PDF using C#

It was observed that an incomplete evaluation message is displaying when customer is using a free version of Aspose.BarCode API. In this release this issue has been addressed. Following is the list of fixes that were reported by our valued customers.

*   Barcode recognition process have been improved to detect barcodes from PDF files. It was reported that Aspose.BarCode is unable to recognize the barcode from PDF. After investigation it was found that PDF file was created in a very strange way. The barcode image has been stored as a bunch of lines (pieces or parts). When we try to extract the barcode image from PDF file using Aspose.PDF (**Aspose.Pdf.Facades.PdfExtractor**) it returns many images instead of a single barcode image due to which Aspose.BarCode APIs were unable to recognize the barcode. For this particular case, it is recommended to convert PDF file pages into a single image format with at least 300-400 DPI.
*   Functionality to recognize barcode from images has been enhanced. An other issue was reported that Aspose.BarCode is unable to recognize barcode from a driving license image. In the detailed investigation, it was found that there is no issue with the Aspose.BarCode functionality. The data in the driver license has a particular format and it depends from country to country and state to state.

To view a complete list of fixes, please visit the [release notes][2] page. You can access **Aspose.Barcode for .NET 18.3** through [Nuget Gallery][3].

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   [Aspose.BarCode for .NET Wiki docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+18.3+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.BarCode/
[4]: https://products.aspose.com/barcode/net
[5]: https://www.nuget.org/packages/Aspose.BarCode/
[6]: https://docs.aspose.com/barcode/net/
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET




