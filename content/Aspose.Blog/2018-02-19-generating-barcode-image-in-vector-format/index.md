---
title: 'Generating Barcode Image In Vector Format With Aspose.BarCode for Java 18.1'
date: Mon, 19 Feb 2018 04:15:25 +0000
draft: false
url: /2018/02/19/generating-barcode-image-in-vector-format/
author: Ikram Haq
summary: ''
tags: ['Generate Barcode Image In Vector Format in Java', 'Java BarCode API']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="Aspose.BarCode for Java">}}


Aspose.BarCode for Java 18.1 is available for [download][1] now. The major development in this release is the support to save the generated barcode image in Vector format. This release also supports the enhanced process of drawing barcode text when the font is specified in the code snippet. The enhanced working of CodeLocation property has also been incorporated in this release.

## Generating Barcode Image In Vector Format

Aspose.BarCode for Java now supports the functionality to generate barcode images in vector format. Two new properties Emf and Svg have been introduced in com.aspose.barcode.BarCodeImageFormat class which can be set before saving barcode image. How a developer can save barcode image in vector format is quite simple and is demonstrated in the code snippet given below. The code snippet contains comments that make it self explanatory.

```
 // Instantiate BarCodeBuilder object
com.aspose.barcode.BarCodeBuilder builder = new com.aspose.barcode.BarCodeBuilder();

// Set the Code text for the barcode
builder.setCodeText("ABCDEFGHIJKLMNOPQRSTUVWXYZ");

// Set the symbology type to QR
builder.setEncodeType(com.aspose.barcode.EncodeTypes.QR);

//Save the image
builder.save("qr_test.emf", com.aspose.barcode.BarCodeImageFormat.Emf); 
```

## Other Improvements

Following is the list of improvements made in this release and bug fixes that were reported by our valued customers.

*   Process of setting license has been improved. Now API will show correct exception message in case license subscription is expired. Set license execution time has also been improved.
*   Inaccurate barcode text was displayed when font is specified while saving the barcode image in vector format. The enhancement has been made to draw barcode text properly.
*   Setting big text size with com.aspose.barcode.StringAlignment.Far option, it was noticed that the barcode text disappears. Now the issue has been fixed.
*   Working of setCodeLocation property has been improved.

To view a complete list of enhancements and fixes, please visit the [release notes][2] page.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java][3]
*   Install Aspose.BarCode for Java from Maven
*   [Download Aspose.BarCode for Java][4]
*   [Aspose.BarCode for Java Wiki docs][5] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-barcode/18.1/
[2]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Java+18.1+-+Release+Notes
[3]: https://products.aspose.com/barcode/java
[4]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-barcode/
[5]: https://docs.aspose.com/display/barcodejava/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




