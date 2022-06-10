---
title: 'Support of Recognition Modes, Unicode Text Detection, Micro PDF417 and Micro QR using Aspose.BarCode for Java 6.9.0'
date: Thu, 09 Jul 2015 17:00:37 +0000
draft: false
url: /2015/07/09/support-of-recognition-modes-unicode-text-detection-micro-pdf417-and-micro-qr-using-aspose.barcode-for-java-6.9.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)We are pleased to announce the release of [Aspose.BarCode for Java 6.9.0][2]. This month's release provides many useful improvements & enhancements where the most worth mentioning feature is the support for various recognition modes that allows the developers to configure the recognition for speed and accuracy. In case you wish to upgrade the Aspose.BarCode for Java API from any previous release, we strongly recommend you to go through the Public API Changes section to know what has been changed in the public API since your current revision of he API.

While you are downloading the latest build of Aspose.BarCode for Java, here is a look at just a few of the showcased features for this release.

## Tune the Speed and Quality with Recognition Modes

Speed and quality are two important factors that always influence each other. Often the developers have to compromise on the one to get the other. With the release of Aspose.BarCode for Java, the API has provided the support to customize the recognition quality and performance while using the Recognition Modes that should help the developers to configure their application for recognition accuracy and speed as per requirements.

## Encoding of Micro PDF417 Code

Micro PDF147 code is the extended form of PDF417 that allows to encode more bytes than PDF147. Micro-PDF417 is designed for applications requiring improved area efficiency. With the release of version 6.9.0, the API allows the generation of Micro-PDF417 whereas the recognition for the said symbology is already available by the Aspose.BarCode for Java API.

## Decoding of Micro QR Code

Micro QR code is a smaller version of the QR code best suited for the applications that impose limit on the symbol size. Aspose.BarCode for Java 6.9.0 has extended its support for recognition of Micro QR codes whereas the encoding is expected to be available with future releases of the API.

## Detect Barcode Unicode Text

Aspose.BarCode for Java 6.9.0 allows the developers to detect the Unicode encoding. In case the detect encoding flag is enabled the barcode engine returns Unicode text while trying to detect the encoding of the barcode using one of the following encoding standards:

*   UTF8BOM
*   UTF8BOM
*   UTF16BEBOM
*   UTF16LE

Please note, the flag is enabled by default. In case the flag is disabled the engine returns plain text without encoding detection.

## Render Barcodes with Empty Outlined Bars

This release has exposed the FilledBars property for the BarCodeBuilder class. This newly exposed property allows to control the filling of the barcode bars. The default value of FilledBars property is true, that means the barcodes are generated with filled bars, however, if set to false the generated barcode will have empty bars with just outlines as shown in the following illustration. Please note, the FilledBars is only applicable for 1D barcodes.

[![][3]](https://blog.aspose.com/wp-content/uploads/sites/2/2015/07/EmptyBars.png)

## Aspose.BarCode for Java Resources

The resources you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][4]
*   [Download Aspose.BarCode for Java][5]
*   Aspose.BarCode for Java Wiki docs - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/entry640117.aspx "Download Aspose.BarCode for Java 6.9.0"
[3]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/07/EmptyBars.png "EmptyBars"
[4]: http://www.aspose.com/java/barcode-component.aspx
[5]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[7]: https://blog.aspose.com/
[8]: https://github.com/asposebarcode/Aspose_BarCode_JAVA




