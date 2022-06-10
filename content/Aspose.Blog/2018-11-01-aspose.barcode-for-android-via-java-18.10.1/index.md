---
title: 'Aspose.BarCode for Android via Java 18.10.1'
date: Thu, 01 Nov 2018 11:22:15 +0000
draft: false
url: /2018/11/01/aspose.barcode-for-android-via-java-18.10.1/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://products.aspose.com/barcode/java)We are pleased to announce the release of [Aspose.BarCode for Android via Java 18.10.1][2]. This release addresses the instance reusability issue of the BarCodeReader. For a detailed note on what is new and fixed, please visit the [release notes][3] page for information of API documentation.

## Enhancements made to the BarCodeReader

Before this release, if you wanted to scan two Barcodes, you had to create a new instance of the BarCodeReader to scan the second Barcode. This release of Aspose.Barcode for Android via Java addresses that issue. Now you can scan multiple Barcodes using the same instance of the BarCodeReader. This is demonstrated using a simple example given below.

```
BarCodeReader reader = new BarCodeReader();  
reader.setBarCodeReadType(DecodeType.ALL\_SUPPORTED\_TYPES);  
reader.setBarCodeImage("Barcode1.jpg");  
while (reader.read())  
{  
    System.out.println("Barcode 1: " \+ reader.getCodeText());  
}  
reader.setBarCodeImage("Barcode2.png");  
while (reader.read())  
{  
    System.out.println("Barcode 2: " \+ reader.getCodeText());  
}  
reader.close();
```

## Aspose.BarCode for Android via Java Resources

As Aspose.Barcode for Android via Java is based on Aspose.Barcode for Java, the following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java][4]
    
*   [Download Aspose.BarCode for Java][5]– Install Aspose.BarCode for Java from Maven
    
*   [Aspose.BarCode for Java Wiki docs][6]– help documentation and API reference documents.
    
*   [Aspose.BarCode Product Family Forum][7]– post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
    
*   [Enable Email Subscription][8]– Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
    
*   [Aspose.BarCode for Java Examples][9]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2018/02/aspose-BarCode-for-Java_100.png
[2]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/18.10.1/aspose-barcode-18.10.1-android.via.java.jar
[3]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Android+via+Java+18.10.1
[4]: https://products.aspose.com/barcode/java
[5]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/
[6]: https://docs.aspose.com/display/barcodejava/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




