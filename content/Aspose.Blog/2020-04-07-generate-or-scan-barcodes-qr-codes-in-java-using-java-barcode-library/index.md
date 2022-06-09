---
title: 'Generate and Scan Barcodes Programmatically using Java'
seoTitle: ""
description: ""
date: Tue, 07 Apr 2020 03:11:00 +0000
draft: false
url: /2020/04/07/generate-or-scan-barcodes-qr-codes-in-java-using-java-barcode-library/
author: Usman Aziz
summary: ''
tags: ['Generate Barcode and QR Code in Java', 'Java barcode generator', 'Java barcode scanner reader', 'Scan and read barcodes in Java']
categories: ['Aspose.BarCode Product Family']
---

In this article, I'll show you how to **generate barcodes programmatically using Java**. Furthermore, you will also learn how to scan and read different types of barcodes using Java.



{{< figure align=center src="images/Generate-Barcode-in-Java-2.png" alt="Generate Barcode in Java 2">}}


**[Barcode][1]** technology is a popular and widely used way to visually represent data about objects in the form of different patterns. Barcode is the encoded and machine-readable form of the data that can be decoded or read using the **barcode scanners**. These days, almost every product contains a barcode that can be scanned to retrieve information about that product. Furthermore, the increasing number of online businesses has also influenced the usage of different types of barcodes in the purchase process. Keeping an eye on today's trends, this article aims to show you how to **generate and scan** various types of **barcodes** within your **Java** applications using Aspose' barcode generator and scanner library.

In this article, you will learn how to:

*   [Generate a barcode using Java][2]
*   [Generate QR or other barcodes using Java][3]
*   [Create barcodes with a customized appearance using Java][4]
*   [Create barcodes with a caption using Java][5]
*   [Scan and read barcodes in Java][6]

## Java Barcode Generator and Scanner Library

In order to generate barcodes in Java-based applications, i.e. console application, Java Swing application, [Aspose.BarCode for Java][7] has proved to be a flexible and feature-rich Java barcode generator and scanner library. You can [download][8] the JAR of Aspose.BarCode for Java or install it in your Maven-based application using the following configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-barcode</artifactId>
    <version>20.3</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Generate a Barcode using Java {#Generate-a-barcode-using-Java}

The following are the simple steps to generate a barcode as an image.

*   Create an object of the [BarcodeGenerator][9] class.
*   Initialize the _BarcodeGenerator_ object with the encoding type and the text to encode.
*   Set the resolution of the resultant image (optional).
*   Generate barcode using [BarcodeGenerator.save(string)][10] method.

The following code sample shows how to generate a barcode using Java.

{{< gist aspose-com-gists 36fb6b6f0ea0341ee24e9713570c2534 "generate-barcode.java" >}}

### Generated Barcode



{{< figure align=center src="images/generate-barcode-java.png" alt="Java Barcode generator library">}}


## Generate QR Barcode using Java {#Generate-QR-or-other-barcodes}

You can generate a variety of barcode types using Aspose.BarCode for Java. The supported barcode symbologies of the API include, but not limited to:

*   Code128
*   Code11
*   Code39
*   QR
*   Datamatrix
*   EAN13
*   EAN8
*   ITF14
*   PDF417
*   and [more][11].

You can generate any of the above-mentioned barcode types by specifying the respective encoding type using the [EncodeTypes][12] parameter while initializing the BarcodeGenerator's object. For the demonstration, we'll generate a QR barcode. The following code sample shows how to generate QR barcode in Java:

{{< gist aspose-com-gists 36fb6b6f0ea0341ee24e9713570c2534 "generate-qr-barcode.java" >}}

### Generated QR Code



{{< figure align=center src="images/generate-qr-barcode-java.png" alt="Java QR barcode generator">}}


## Generate Customized Barcode using Java {#Create-barcodes-with-a-customized-appearance}

By default, the barcodes are generated in black and white color combination. However, in certain cases, you may want or need to customize its appearance. Aspose.BarCode for Java lets you customize the barcode's forecolor, back color, text's color, font, and etc. The following is the recipe to generate a customized barcode.

*   Create an object of the [BarcodeGenerator][13] class.
*   Initialize _BarcodeGenerator_ with the encoding type and the text to encode.
*   Access and set the parameters related to the appearance of the barcode using [BarcodeGenerator.getParameters()][14].
*   Generate barcode using [BarcodeGenerator.save(string)][15] method.

The following code sample shows how to generate an AZTEC barcode with a customized appearance using Java.

{{< gist aspose-com-gists 36fb6b6f0ea0341ee24e9713570c2534 "generate-barcode-custom.java" >}}

### Barcode with Customized Appearance



{{< figure align=center src="images/generate-barcode-custom-appearance.png" alt="java generate aztec barcode ">}}


## Generate Barcodes with Captions in Java {#Create-barcodes-with-a-caption}

The barcode images may also contain their captions. You can add the caption below the barcode, above the barcode, or at both of the locations at the same time. The following steps are used to set captions for a barcode:

*   Create an object of the [BarcodeGenerator][16] class and initialize it with the encoding type and the code text.
*   Access and set the captions using [BarcodeGenerator.getParameters().getCaptionAbove().setText()][17] or [getCaptionBelow().setText()][18] methods.
*   Set the visibility of the captions using the _setVisible()_ method.
*   Generate barcode using [BarcodeGenerator.save(string)][19] method.

The following code sample shows how to generate a barcode with the caption in Java.

{{< gist aspose-com-gists 36fb6b6f0ea0341ee24e9713570c2534 "generate-barcode-with-caption.java" >}}

### Barcode with Captions



{{< figure align=center src="images/generate-barcode-with-caption-java.png" alt="generate barcode with caption">}}


## Read or Scan Barcode in Java {#Scan-and-read-barcodes-in-Java}

Along with generating the barcodes, you can also scan the barcode images to decode and read the information/data they contain. Since an image may contain more than one barcode, you may access and read all of them at the same time. The following are the steps to scan and read a barcode image:

*   Create an object of [BarCodeReader][20] class and initialize it with the path of the barcode image file.
*   You can also pass [DecodeType][21] as the second parameter to BarCodeReader's constructor to read the barcodes with a particular symbology only.
*   Read the barcodes using [BarCodeReader.readBarCodes()][22] method.

The following code sample shows how to scan and read barcode images in Java.

{{< gist aspose-com-gists 36fb6b6f0ea0341ee24e9713570c2534 "scan-read-barcode.java" >}}

### Output```
CodeText: Aspose.BarCode
Symbology type: Code128
```

## Conclusion

In this article, we have seen how to generate different types of barcodes using Java. The step by step guide and code samples demonstrated how to customize the barcode's appearance and scan the barcodes within Java applications. You can explore more about Aspose.BarCode for Java using its [documentation][23].

## Related Articles

*   [PHP Barcode Generator and Reader API][24]




[1]: https://en.wikipedia.org/wiki/Barcode
[2]: #Generate-a-barcode-using-Java
[3]: #Generate-QR-or-other-barcodes
[4]: #Create-barcodes-with-a-customized-appearance
[5]: #Create-barcodes-with-a-caption
[6]: #Scan-and-read-barcodes-in-Java
[7]: https://products.aspose.com/barcode/java
[8]: https://downloads.aspose.com/barcode/java
[9]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator
[10]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator#save-java.lang.String-
[11]: https://docs.aspose.com/display/barcodejava/Barcode+Supported+Symbologies
[12]: https://apireference.aspose.com/
[13]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator
[14]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator#getParameters--
[15]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator#save-java.lang.String-
[16]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator
[17]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BaseGenerationParameters#getCaptionAbove--
[18]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BaseGenerationParameters#getCaptionBelow--
[19]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.generation/BarcodeGenerator#save-java.lang.String-
[20]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeReader
[21]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/DecodeType
[22]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeReader#readBarCodes--
[23]: https://docs.aspose.com/display/barcodejava/Product+Overview
[24]: https://blog.aspose.com/2020/01/29/php-barcode-generator-reader-and-scanner-api/





