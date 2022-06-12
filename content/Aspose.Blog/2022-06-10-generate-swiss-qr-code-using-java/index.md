---
title: 'Generate Swiss QR Code using Java'
seoTitle: "Generate Swiss QR Code using Java | Read Swiss QR Code in Java"
description: "Programmatically generate, decode and read Swiss QR Code using Java with Aspose.BarCode for Java API. Generate complex barcodes using Java."
date: Fri, 10 Jun 2022 09:17:28 +0000
draft: false
url: /2022/06/10/generate-swiss-qr-code-using-java/
author: Muzammil Khan
summary: 'The Swiss QR Code encodes all the necessary payment information required to trigger payments. In this article, you will learn **how to generate a Swiss QR Code, decode and read payment information from a Swiss QR code using Java**.'
tags: ['Generate QR Code in Java', 'Generate QR Codes', 'Java API to Generate Swiss QR Code', 'Read Swiss QR Code', 'Read Swiss QR Code in Java', 'Swiss QR Bill', 'Swiss QR Bill Generator', 'Swiss QR Code', 'Swiss QR Code Generator']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/generate-swiss-qr-code-using-java.jpg" alt="Generate Swiss QR Code using Java">}}


A Swiss QR code is also known as the Swiss QR Bill. It was developed to automate digital payments. We can easily encode all the necessary payment information required to trigger payments in the Swiss QR Code. The Swiss QR code contains a Swiss cross in the middle. In this article, we will learn **how to generate a Swiss QR Code using Java**. Furthermore, we will also learn **how to decode and read payment information from a Swiss QR code** programmatically.

The following topics shall be covered in this article:

*   [Java API to Generate and Read Swiss QR Code][1]
*   [Generate Swiss QR Code][2]
*   [Customize Swiss QR Code][3]
*   [Read Swiss QR Code][4]

## Java API to Generate and Read Swiss QR Code {#Java-API-to-Generate-and-Read-Swiss-QR-Code}

For generating and reading Swiss QR codes, we will be using the _[Aspose.BarCode for Java][5]_ API. It provides _[SwissQRBill][6]_ and _[SwissQRCodetext][7]_ classes offering various properties to work with Swiss QR codes. The _SwissQRBill_ class enables getting or setting billing and payment data, such as account information, amount, currency, and creditor details. The _SwissQRCodetext_ class allows encoding and decoding of the _SwissQRBill_ information embedded in the Swiss QR code.

The API provides the _[ComplexBarcodeGenerator][8]_ class for generating images of complex barcodes, such as Swiss QR codes. The _[BarCodeReader][9]_ class of the API allows reading the barcodes of the specified _[DecodeType][10]_. The [_BarCodeResult_][11] class of the API stores the recognized barcode data, such as barcode type and code text. Moreover, it is a feature-rich API that lets you generate, scan, and read a wide range of [barcode symbologies][12].

Please either [download][13] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

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

## Generate Swiss QR Code in Java {#Generate-Swiss-QR-Code-in-Java}

We can generate a Swiss QR code by following the steps given below:

*   Create an instance of the **_SwissQRCodetext_** class.
*   Set various **_SwissQRBill_** properties such as Version, Account, Amount, Currency, Reference, etc.
*   Initialize the **_Address_** class objects and set Creditor and Debtor details.
*   After that, create an instance of the **_ComplexBarcodeGenerator_** class with the **_SwissQRCodetext_** object.
*   Finally, call the [save()][14] method to save the image at the given file path.

The following code sample shows **how to generate a Swiss QR code using Java**.

\[gist id="fc2a200a89a9333a1fbccd9e640f2638" file="Generate-Swiss-QR-Code-Java\_Generate.java"\]



{{< figure align=center src="images/SwissQRBill-1.png" alt="" caption="Generate Swiss QR Code in Java.">}}


## Customize Swiss QR Code in Java {#Customize-Swiss-QR-Code-in-Java}

We can customize the appearance of a Swiss QR code by following the steps given below:

*   Create an instance of the **_SwissQRCodetext_** class.
*   Set various **_SwissQRBill_** properties such as Version, Account, Amount, Currency, Reference, etc.
*   Initialize the **_Address_** class objects and set Creditor and Debtor details.
*   Create an instance of the **_ComplexBarcodeGenerator_** class with the **_SwissQRCodetext_** object.
*   After that, set various barcode parameters such as image width, encoding, back color, resolution, border, etc.
*   Finally, call the [save()][15] method to generate the code. It takes the image file path and **_BarCodeImageFormat_** as arguments.

The following code sample shows **how to customize a Swiss QR code using Java**.

\[gist id="fc2a200a89a9333a1fbccd9e640f2638" file="Generate-Swiss-QR-Code-Java\_Customize.java"\]



{{< figure align=center src="images/SwissQRBill-1.jpg" alt="Customize Swiss QR Code in Java" caption="Customize Swiss QR Code in Java">}}


## Read Swiss QR Code in Java {#Read-Swiss-QR-Code-in-Java}

We can read barcodes from an image by following the steps given below:

*   Firstly, load an image using the **_BarCodeReader_** class.
*   Get recognition results in **_BarCodeResult_** class object using the **_readBarCodes()_** method.
*   Loop through the results and decode the Swiss QR code using the **_tryDecodeSwissQR()_** method.
*   Finally, read the **_SwissQRCodetext_** and show the data.

The following code sample shows how to **read a Swiss QR code from an image using Java**.

\[gist id="fc2a200a89a9333a1fbccd9e640f2638" file="Generate-Swiss-QR-Code-Java\_Read.java"\]

```
Version: V2_0
Account: CH4431999123000889012
Amount: 1000.25
Currency: CHF
Reference: 210000000003139471430009017
Creditor Name: Muster & Söhne
Creditor Street: Musterstrasse
Creditor House: 12b
Creditor Postal Code: 8200
Creditor Town: Zürich
Creditor Country: CH
Debtor Name: Muster AG
Debtor Street: Musterstrasse
Debtor House: 1
Debtor Postal Code: 3030
Debtor Town: Bern
Debtor Country: CH 
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][16] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   generate Swiss QR Bill image programmatically;
*   set QR code image size and resolution;
*   set the border and back color of the QR code;
*   detect a Swiss QR code from an image;
*   read payment details from the Swiss QR Code in Java.

Besides, you can learn more about **_Aspose.BarCode for Java_** API using the [documentation][17]. In case of any ambiguity, please feel free to contact us on the [forum][18].

## See Also

*   [Generate Barcodes using Java][19]
*   [Read Barcode from Image using Java][20]


[1]: #Java-API-to-Generate-and-Read-Swiss-QR-Code
[2]: #Generate-Swiss-QR-Code-in-Java
[3]: #Customize-Swiss-QR-Code-in-Java
[4]: #Read-Swiss-QR-Code-in-Java
[5]: https://products.aspose.com/barcode/java/
[6]: https://reference.aspose.com/barcode/java/com.aspose.barcode.complexbarcode/SwissQRBill
[7]: https://reference.aspose.com/barcode/java/com.aspose.barcode.complexbarcode/SwissQRCodetext
[8]: https://reference.aspose.com/barcode/java/com.aspose.barcode.complexbarcode/ComplexBarcodeGenerator
[9]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeReader
[10]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/DecodeType
[11]: https://apireference.aspose.com/barcode/java/com.aspose.barcode.barcoderecognition/BarCodeResult
[12]: https://docs.aspose.com/barcode/java/barcode-supported-symbologies/
[13]: https://downloads.aspose.com/barcode/java
[14]: https://reference.aspose.com/barcode/java/com.aspose.barcode.complexbarcode/ComplexBarcodeGenerator#save-java.lang.String-
[15]: https://reference.aspose.com/barcode/java/com.aspose.barcode.complexbarcode/ComplexBarcodeGenerator#save-java.lang.String-com.aspose.barcode.generation.BarCodeImageFormat-
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/barcode/java/
[18]: https://forum.aspose.com/c/barcode/13
[19]: https://blog.aspose.com/2020/04/07/generate-or-scan-barcodes-qr-codes-in-java-using-java-barcode-library/
[20]: https://blog.aspose.com/2022/06/04/read-barcode-from-image-using-java/





