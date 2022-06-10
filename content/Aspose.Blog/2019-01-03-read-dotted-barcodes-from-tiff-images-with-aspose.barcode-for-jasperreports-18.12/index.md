---
title: 'Read Dotted BarCodes from TIFF Images in JasperReports'
date: Thu, 03 Jan 2019 21:37:24 +0000
draft: false
url: /2019/01/03/read-dotted-barcodes-from-tiff-images-with-aspose.barcode-for-jasperreports-18.12/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-JasperReports_100.png" alt="Aspose.BarCode for JasperReports">}}


We are pleased to announce the release of Aspose.BarCode for JasperReports 18.12. This release gives you the ability to read dotted barcodes from Tiff images.  
To view a complete list of fixes, please visit [Aspose.Barcode for JasperReport 18.12 release notes][1] page.

## Read Dotted BarCodes from TIFF Images in Jasper Reports

The new release of Aspose.BarCode adds the ability to read dotted barcodes from Tiff images. You may read such barcodes as shown below.

```
String fileName = "Test.tiff";  
BarCodeReader reader = new BarCodeReader(fileName,   
new MultyDecodeType(DecodeType.ALL\_SUPPORTED\_TYPES));  
while (reader.read())  
    System.out.println(reader.getCodeText());
```

## Other Enhancements made to the API

Other than the ability to read dotted barcodes from Tiff images, XML serialization was enhanced and made compatible between .NET and Java.

You can download the latest release of Aspose.BarCode for JasperReports from the following link:

*   [Download Aspose.BarCode for JasperReports 18.12.][2]

## Aspose.BarCode for JasperReports Resources

The following API resources can be of help to you in getting started:

*   [Homepage for Aspose.BarCode for JasperReports API][3]
*   [Download Aspose.BarCode for JasperReports][4]
*   [Aspose.BarCode for JasperReports Wiki docs][5] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://docs.aspose.com/display/barcodejasperreports/Aspose.BarCode+for+JasperReports+18.12+-+Release+notes
[2]: https://downloads.aspose.com/barcode/jasperreports/new-releases/aspose.barcode-for-jasperreports-18.12/
[3]: https://products.aspose.com/barcode/jasperreports
[4]: https://downloads.aspose.com/barcode/jasperreports
[5]: https://docs.aspose.com/display/barcodejasperreports/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




