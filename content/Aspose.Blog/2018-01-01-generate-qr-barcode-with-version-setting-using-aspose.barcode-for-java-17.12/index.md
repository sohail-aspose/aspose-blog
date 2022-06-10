---
title: 'Generate QR Barcode with Version Setting Using Aspose.BarCode for Java 17.12'
date: Mon, 01 Jan 2018 19:42:38 +0000
draft: false
url: /2018/01/01/generate-qr-barcode-with-version-setting-using-aspose.barcode-for-java-17.12/
author: Ikram Haq
summary: ''
tags: ['Create QR code in Java', 'Generate QR barcode in Java', 'Java BarCode API', 'Java Barcode generator library', 'QR Code Generator in Java']
categories: ['Aspose.BarCode Product Family']
---

Aspose.BarCode for Java 17.12 is available for [download][1] now. The major development in this release is the support to [generate QR coded barcode with its version number][2]. This release also supports enhanced process of recognizing Code128 and OneD coded barcode. Enhanced speed and quality of 1D barcode recognition process functionality has also been incorporated in this release.

## Setting QR version

Aspose.BarCode for Java now supports the functionality to [generate QR coded barcode with its version information][3]. This functionality allows the developers to generate QR coded barcode by setting its version number. A property BarCodeBuilder.setQRVersion has been introduced to define the said setting. How a developer can set QR version number is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

```
// Instantiate BarCodeBuilder object
com.aspose.barcode.BarCodeBuilder builder = new com.aspose.barcode.BarCodeBuilder();

// Set the Code text for the barcode
builder.setCodeText("ABCDEFGHIJKLMNOPQRSTUVWXYZ");

// Set the symbology type to QR
builder.setEncodeType(com.aspose.barcode.EncodeTypes.QR);

// Set the error level
builder.setQRErrorLevel(com.aspose.barcode.QRErrorLevel.LevelQ);

// Set the QR barcode version number
builder.setQRVersion(com.aspose.barcode.QRVersion.VERSION_10);

//Save the image
builder.save("qr_version10_errorQ.png");
```

## Other Improvements

Following is the list of improvements made in this release and bug fixes that were reported by our valued customers.

*   Process of setting license has been improved. Now API will show correct exception message in case license subscription is expired. Set license execution time has also been improved.
*   Working of Aspose.BarCode in multi threaded environment has been enhanced.
*   DatabarStacked barcode recognition process has been enhanced.
*   Process of recognizing barcode from JPEG and TIFF image has been improved.
*   Functionality to generate Datamatrix barcode has been updated.
*   Process to recognize PDF417 and Code128 barcode has been enhanced. Performance improvements have been made to boost up the process.

To view a complete list of enhancements and fixes, please visit the [release notes][4] page.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java API][5]
*   [Download Aspose.BarCode for Java][6]
*   [Aspose.BarCode for Java Wiki docs][7] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][8] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][9] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][10] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/barcode/java
[2]: https://docs.aspose.com/display/barcodejava/Creating+a+QR+Barcode#CreatingaQRBarcode-HowtosetQRversion
[3]: https://docs.aspose.com/display/barcodejava/Creating+a+QR+Barcode#CreatingaQRBarcode-HowtosetQRversion
[4]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Java+17.12+-+Release+Notes
[5]: https://products.aspose.com/barcode/java
[6]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-barcode/
[7]: https://docs.aspose.com/display/barcodejava/Home
[8]: https://forum.aspose.com/c/barcode
[9]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[10]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




