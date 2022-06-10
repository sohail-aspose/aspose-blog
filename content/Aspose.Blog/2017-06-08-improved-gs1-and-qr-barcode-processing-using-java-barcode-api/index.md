---
title: 'Enhanced GS1 and QR Barcode Processing using Java Barcode API'
date: Thu, 08 Jun 2017 11:16:08 +0000
draft: false
url: /2017/06/08/improved-gs1-and-qr-barcode-processing-using-java-barcode-api/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose_barcode-for-java.jpg" alt="">}}


Aspose.Barcode for Java 17.4 has been released. The major development in this release is the enhanced functionality of GS1 coded barcode. GS1 code format can contain complex elements with digits and letters. Enhanced GS1 barcode functionality now can parse and validate these complex combinations. Improved QR coded barcode recognition functionality has also been incorporated in this release.

## Enhanced GS1 Barcode Processing using Java

Aspose.BarCode for Java now generates AI **(Application Identifier)** compliance GS1 coded barcode. Checksum calculation and validation for many AI specifications have been implemented. As an example, consider code text **“(703)123”**, this is an incorrect code text (ref: 703 AI, with letters - 324a, with more than 4 symbols). Aspose.BarCode will generates exception if user tries to generate the barcode with **EncodeTypes** as **GS1Code128**. The following exception message will be displayed for such an incorrect barcode.

### Exception Message:

Wrong format of GS1 Code128 input string.

## Improved QR Barcode Processing using Java

Targets detection logic for **QR** coded barcode has been updated. Aspose.BarCode for Java can now detect **QR** coded barcode in combination with **MaxQuality** mode for better accuracy. The said functionality is as illustrated in the following code sample.

```
 //Initialize reader object
com.aspose.barcode.barcoderecognition.BarCodeReader reader = new com.aspose.barcode.barcoderecognition.BarCodeReader("sample_QR_barcode.bmp", com.aspose.barcode.barcoderecognition.DecodeType.QR);

// Set recognition mode to MaxQuality
reader.setRecognitionMode(com.aspose.barcode.barcoderecognition.RecognitionMode.MaxQuality);

// Read the barcode
while (reader.read())
{
    // print output
    System.out.println("Type : " + reader.getCodeType());
    System.out.println("Code Text : " + reader.getCodeText());
} 
```

## Enhancements

The complete list of enhancements and fixes in this release is as follows.

*   Recognition process of QR barcode in MaxBarCodes mode has been improved.
*   Functionality of ExportToXml method has been improved. ExportToXml method now export dimension properties along with other properties of the newly define barcode into XML file.

To view a complete list of new features, fixes and to download the latest release, please visit [Aspose.Barcode for Java 17.4][1] page in downloads section.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java API][2]
*   [Download Aspose.BarCode for Java][3]
*   [Aspose.BarCode for Java Wiki docs][4] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][5] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][6] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][7] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/barcode/java
[2]: https://www.aspose.com/products/barcode/java
[3]: https://downloads.aspose.com/barcode/java
[4]: https://docs.aspose.com/display/barcodejava/Home
[5]: https://forum.aspose.com/c/barcode
[6]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[7]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




