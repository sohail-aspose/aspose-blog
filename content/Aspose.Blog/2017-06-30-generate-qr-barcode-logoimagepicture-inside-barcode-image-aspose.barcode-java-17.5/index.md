---
title: 'Generate QR Barcode with Logo/Image/Picture using Java'
date: Fri, 30 Jun 2017 05:25:12 +0000
draft: false
url: /2017/06/30/generate-qr-barcode-logoimagepicture-inside-barcode-image-aspose.barcode-java-17.5/
author: Ikram Haq
summary: ''
tags: ['Generate C40 encoded datamatrix barcode Java', 'Generate QR barcode with image in Java', 'Generate QR barcode with logo in Java', 'Generate text encoded datamatrix barcode java']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="">}}


We are pleased to announce the release of Aspose.Barcode for Java 17.5. The major development in this release is the support to [generate the QR barcode with a logo/image inside the barcode image][1]. This release supports [generating DataMatix barcode with C40 and Text encoding scheme][2]Barcodes-CreateC40EncodedDatamatrixBarcode). The functionality of AllSupportedTypes recognition mode has also been improved and incorporated in this release.

## Create QR Barcode with Image in Java

Aspose.BarCode now supports [generating QR barcode with logo/other image inside][3] it. How a developer can embed a logo/image/picture inside a QR barcode image is very simple and is demonstrated in the code snippet given below. The code snippet is ornate with comments that make it self explanatory.

{{< gist aspose-com-gists 9dea2dd38be50330a824dd05da062a97 "Examples-src-main-java-com-aspose-barcode-examples-TwoD_barcodes-basic_features-CreatingAQRBarcode-QRBarcodeWithImage.java" >}}

## Create C40 Encoded Datamatrix Barcode

Aspose.BarCode for Java provides the most convenient way to produce C40 encoded DataMatrix. How simple it is to [produce a C40 encoded DataMatrix][4]Barcodes-CreateC40EncodedDatamatrixBarcode) is illustrated in the following code sample.

{{< gist aspose-com-gists 9dea2dd38be50330a824dd05da062a97 "Examples-src-main-java-com-aspose-barcode-examples-TwoD_barcodes-basic_features-CreateDatamatrixBarcode-createDataMatrixBarcodeWithC40Encoding.java" >}}

## Create Text Encoded Datamatrix Barcode

Aspose.BarCode for Java provides the functionality to generate the DataMatrix barcode with a Text encoding scheme. Following code snippet demonstrates how to create DataMatrix with Text mode enabled.

```
// Create an instance of BarCodeBuilder class
// Set codetext value and EncodeType
com.aspose.barcode.BarCodeBuilder buidler = new com.aspose.barcode.BarCodeBuilder("ABCDEF123456", com.aspose.barcode.EncodeTypes.DATA_MATRIX);

// Set the DataMatrix encoding mode to Text
buidler.setDataMatrixEncodeMode(com.aspose.barcode.DataMatrixEncodeMode.TEXT);

// Save the barcode image
buidler.save("dataMatrixC40.png");
```

## Enhancements

The complete list of enhancements and fixes in this release is as follows.

*   The functionality of AllSupportedTypes recognition mode has been improved.
*   The functionality to recognize DataMatix barcode has been improved. Recognition algorithm has been improved in such a way that it is now capable of decoding non-printable chars and decoding some special characters/symbols.
*   Functionality to read barocde from PDF file has been improved.

To view a complete list of new features, fixes and to download the latest release, please visit [Aspose.Barcode for Java 17.5][5] page in downloads section.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java API][6]
*   [Download Aspose.BarCode for Java][7]
*   [Aspose.BarCode for Java Wiki docs][8] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][9] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][10] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][11] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/barcodejava/Creating+a+QR+Barcode#CreatingaQRBarcode-CreateQRBarcodewithLogo
[2]: https://docs.aspose.com/display/barcodejava/Creating+Two+Dimensional+%282D%29+Barcodes#CreatingTwoDimensional(2D
[3]: https://docs.aspose.com/display/barcodejava/Creating+a+QR+Barcode#CreatingaQRBarcode-CreateQRBarcodewithLogo
[4]: https://docs.aspose.com/display/barcodejava/Creating+Two+Dimensional+%282D%29+Barcodes#CreatingTwoDimensional(2D
[5]: https://downloads.aspose.com/barcode/java
[6]: https://products.aspose.com/barcode/java
[7]: https://downloads.aspose.com/barcode/java
[8]: https://docs.aspose.com/display/barcodejava/Home
[9]: https://forum.aspose.com/c/barcode
[10]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[11]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




