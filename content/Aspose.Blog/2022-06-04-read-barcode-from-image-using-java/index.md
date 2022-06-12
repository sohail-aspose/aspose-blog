---
title: 'Read Barcode from Image using Java'
seoTitle: "Read Barcode from Image using Java | Java Barcode Reader API"
description: "Programmatically read Barcode from Image using Java with Aspose.BarCode for Java API. Recognize and read multiple barcodes from an image using Java."
date: Sat, 04 Jun 2022 09:52:45 +0000
draft: false
url: /2022/06/04/read-barcode-from-image-using-java/
author: Muzammil Khan
summary: 'As a Java developer, you can easily recognize and read various types of barcodes in Java applications. In this article, you will learn **how to read barcodes from an image using Java.**'
tags: ['Barcode Reader', 'Barcode Reader Definition', 'Java BarCode API', 'Java Barcode Reader', 'Java Barcode Reader API', 'Read Barcode Types in Java', 'Read Barcode from Image', 'Read Barcode from Image Java', 'Read Barcode in Java', 'Read Barcodes using Java', 'Read Multiple Barcodes in Java']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/read-barcode-from-image-using-java.jpg" alt="Read Barcode from Image using Java">}}


Barcodes play a vital role in the accurate tracking of inventory and delivery of products from manufacturing to point of sale. In certain cases, we may need to read barcodes from images programmatically. We can easily detect, recognize and, read various types of barcodes and QR codes in Java applications. It helps to develop barcode reader or scanner applications. In this article, we will learn **how to read a barcode from an image using Java**.

The following topics shall be covered in this article:

*   [What is Barcode][1]
*   [Java API to Read Barcode from Image][2]
*   [Read Barcode from an Image][3]
*   [Recognize Barcode of Specific Type][4]
*   [Read Multiple Barcodes from an Image][5]
*   [Get X and Y Coordinates of Barcode][6]
*   [Read Barcode From Specific Region of Image][7]

## What is Barcode {#What-is-Barcode}

A barcode is a machine-readable code that represents encoded data in the form of numbers and a pattern of parallel lines. The barcode image shows a series of parallel black and white bars varying the widths, spacing, and sizes. Barcode readers or scanners scan the barcode images and decode the information.

## Java API to Read Barcode from Image {#Java-API-to-Read-Barcode-from-Image}

In order to read the barcodes from images within the Java applications, we will be using the [Aspose.BarCode for Java][8]. It is a feature-rich API that lets you generate, scan, and read a wide range of [barcode symbologies][9]. The _[BarCodeReader][10]_ class of the API allows reading the barcodes. The _[readBarCodes()][11]_ method of this class returns an array of recognized [_barcode_s][12]. The API allows reading barcodes of the specified _[DecodeType][13]_. The [_BarCodeResult_][14] class of the API stores the recognized barcode data such as barcode type, code text, region, and other parameters.

Please either [download][15] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-barcode</artifactId>
    <version>22.5</version>
</dependency>
```

## Read Barcode from an Image in Java {#Read-Barcode-from-an-Image-in-Java}

We can read barcodes from an image by following the steps given below:

*   Firstly, load an image using the **_BarCodeReader_** class.
*   Get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Finally, loop through the results and show the barcode’s type and text.

The following code sample shows how to **read a barcode from an image using Java**.

\[gist id="9398f46bb53c789f08868c52a2138a68" file="Read-Barcode-from-Image-Java\_Read.java"\]



{{< figure align=center src="images/Read-Barcode-from-an-Image-in-Java.jpg" alt="Read Barcode from an Image." caption="Read barcode from an image in Java.">}}


## Recognize Barcode of Specific Type in Java {#Recognize-Barcode-of-Specific-Type-in-Java}

We can read a barcode of a specific type from an image by following the steps given below:

*   Firstly, read buffer data of an image file using the **_ImageIO.read()_** method.
*   Next, create an instance of the **_BarCodeReader_** class with a buffered image and Decode Type.
*   Then, set a barcode decode type to read the barcode of a specific type, such as _**CODE\_39\_STANDARD**_.
*   After that, get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Finally, loop through the results and show the barcode’s type and text.

The following code sample shows **how to read a barcode of a specific type from an image using Java**.

\[gist id="9398f46bb53c789f08868c52a2138a68" file="Read-Barcode-from-Image-Java\_ReadSpecificBarcodeType.java"\]



{{< figure align=center src="images/Recognize-Barcode-of-Specific-Type-in-Java.jpg" alt="Recognize Barcode of Specific Type." caption="Recognize the barcode of a specific type in Java.">}}


## Read Multiple Barcodes from Image in Java {#Read-Multiple-Barcodes-from-Image-in-Java}

We can also read all the available barcodes from an image by following the steps given below:

*   Firstly, load an image using the **_BarCodeReader_** class.
*   Next, set a barcode decode type as _**ALL\_SUPPORTED\_TYPES**_.
*   After that, get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Finally, loop through the results and show the barcode’s type and text.

The following code sample shows **how to read multiple barcodes from an image using Java**.

\[gist id="9398f46bb53c789f08868c52a2138a68" file="Read-Barcode-from-Image-Java\_ReadMultipleBarcodes.java"\]



{{< figure align=center src="images/Read-Multiple-Barcodes-from-Image-in-Java.jpg" alt="Read Multiple Barcodes from Image." caption="Read multiple barcodes from an image.">}}


## Get X and Y Coordinates of Barcode using Java {#Get-X-and-Y-Coordinates-of-Barcode-using-Java}

We can read the X and Y coordinates of the detected barcode from an image by following the steps given below:

*   Firstly, load an image using the **_BarCodeReader_** class.
*   Next, get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Then, loop through the results and check if the **_getRegion()_** is not null.
*   After that, get the Points array bounding the barcode region using the **_getPoints()_**.
*   Finally, show the barcode's X and Y points.

The following code sample shows **how to get the X and Y coordinate points of a barcode from an image using Java**.

\[gist id="9398f46bb53c789f08868c52a2138a68" file="Read-Barcode-from-Image-Java\_ReadXY.java"\]



{{< figure align=center src="images/Get-X-and-Y-Coordinates-of-Barcode-using-Java.jpg" alt="Get X and Y Coordinates of Barcode." caption="Get X and Y coordinates of a barcode from an image.">}}


## Read Barcode From Specific Region of Image in Java {#Read-Barcode-From-Specific-Region-of-Image-in-Java}

We can read a barcode from a specific region or an area of an image by following the steps given below:

*   Firstly, read buffer data of an image file using the **_ImageIO.read()_** method.
*   Next, create an instance of the **_BarCodeReader_** class. It takes a buffered image, a rectangle area, and a Decode Type as arguments.
*   After that, get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Finally, loop through the results and show the barcode’s type and text.

The following code sample shows **how to read a barcode from a specific region of an image using Java**.

\[gist id="9398f46bb53c789f08868c52a2138a68" file="Read-Barcode-from-Image-Java\_ReadSpecificRegion.java"\]



{{< figure align=center src="images/Read-Barcode-From-Specific-Region-of-Image-in-Java.jpg" alt="Read Barcode From Specific Region of Image." caption="Read barcodes from a specific region of an image in Java.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][16] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   Load barcode image programmatically;
*   recognize barcodes of different types from an image;
*   read barcode coordinates in Java;
*   detect and read multiple barcodes from a single image;
*   detect and read barcodes from a specific area of an image.

Besides, you can learn more about **_Aspose.BarCode for Java_** API using the [documentation][17]. In case of any ambiguity, please feel free to contact us on the [forum][18].

## See Also

*   [Generate Barcodes using Java][19]


[1]: #What-is-Barcode
[2]: #Java-API-to-Read-Barcode-from-Image
[3]: #Read-Barcode-from-an-Image-in-Java
[4]: #Recognize-Barcode-of-Specific-Type-in-Java
[5]: #Read-Multiple-Barcodes-from-Image-in-Java
[6]: #Get-X-and-Y-Coordinates-of-Barcode-using-Java
[7]: #Read-Barcode-From-Specific-Region-of-Image-in-Java
[8]: https://products.aspose.com/barcode/java
[9]: https://docs.aspose.com/barcode/java/barcode-supported-symbologies/
[10]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeReader
[11]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeReader#readBarCodes--
[12]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeResult
[13]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/DecodeType
[14]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeResult
[15]: https://downloads.aspose.com/barcode/java
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/barcode/java/
[18]: https://forum.aspose.com/c/barcode/13
[19]: https://blog.aspose.com/2020/04/07/generate-or-scan-barcodes-qr-codes-in-java-using-java-barcode-library/





