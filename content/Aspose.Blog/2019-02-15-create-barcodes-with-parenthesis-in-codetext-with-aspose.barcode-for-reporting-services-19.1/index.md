---
title: 'Create Barcodes with parenthesis in CodeText with Aspose.BarCode for Reporting Services 19.1'
date: Fri, 15 Feb 2019 12:09:44 +0000
draft: false
url: /2019/02/15/create-barcodes-with-parenthesis-in-codetext-with-aspose.barcode-for-reporting-services-19.1/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://products.aspose.com/barcode/net)We are pleased to announce the release of Aspose.Barcode for Reporting Services 19.1. This release enhanced the **BarCodeGenerator** API to support parenthesis in the **CodeText**. For a detailed note on what is new and fixed, please visit the [release notes][2] page for information of the API documentation.

## Support for parenthesis in CodeText

This release of Aspose.BarCode enhanced the **BarCodeGenerator** API to allow the **CodeText** to contain parenthesis. You may generate barcodes with parenthesis in the **CodeText** as shown below in the code example. 

```
Aspose.BarCode.Generation.BarCodeGenerator generator = new  
Aspose.BarCode.Generation.BarCodeGenerator(  
Aspose.BarCode.Generation.EncodeTypes.Pdf417);  
  
generator.CodeText = "Sample.Code.Text(Example).20181203\_150435";  
  
generator.Save(TestDirectory + "barcodeTest.png", BarCodeImageFormat.Png);
```

You can download the latest version of Aspose.BarCode for Reporting Services by visiting the [Aspose.BarCode for Reporting Services 19.1][3] page in the downloads section.

## Aspose.BarCode for Reporting Services Resources

You can get started with Aspose.BarCode for Reporting Services by making use of information available in the following:

*   [Homepage for Aspose.BarCode for SSRS API][4]
*   [Download Aspose.BarCode for SSRS][5]
*   [Aspose.BarCode for SSRS Wiki docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose_barcode-for-reporting-services_100.png
[2]: https://docs.aspose.com/display/barcodereportingservices/Aspose.BarCode+for+Reporting+Services+19.1+Release+Notes
[3]: https://downloads.aspose.com/barcode/reportingservices/new-releases/aspose.barcode-for-reporting-services-19.1/
[4]: https://www.aspose.com/products/barcode/reporting-services
[5]: https://downloads.aspose.com/barcode/reportingservices
[6]: https://docs.aspose.com/display/barcodereportingservices/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




