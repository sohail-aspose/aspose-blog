---
title: 'Read Dotted BarCodes from TIFF Images using Java'
date: Thu, 03 Jan 2019 21:36:20 +0000
draft: false
url: /2019/01/03/read-dotted-barcodes-from-tiff-images-with-aspose.barcode-for-java-18.12/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for Java 18.12][1]. This release gives you the ability to read dotted barcodes from Tiff images. For a detailed note on what is new and fixed, please visit the [release notes][2] page of API documentation.

## Read dotted BarCodes from TIFF Images using Java

The new release of Aspose.BarCode adds the ability to read dotted barcodes from Tiff images. You may read such barcodes as shown below.

```
String fileName = "Test.tiff";
BarCodeReader reader = new BarCodeReader(fileName, 
new MultyDecodeType(DecodeType.ALL_SUPPORTED_TYPES));
while (reader.read())
    System.out.println(reader.getCodeText());
```

## Other Enhancements made to the API

Other than the ability to read dotted barcodes from Tiff images, XML serialization was enhanced and made compatible between .NET and Java.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java][3]
*   [Download Aspose.BarCode for Java][4] – Install Aspose.BarCode for Java from Maven
*   [Aspose.BarCode for Java docs][5] – help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/18.12
[2]: https://docs.aspose.com/barcode/java/aspose-barcode-for-java-18-12-release-notes/
[3]: https://products.aspose.com/barcode/java
[4]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/
[5]: https://docs.aspose.com/barcode/java/
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




