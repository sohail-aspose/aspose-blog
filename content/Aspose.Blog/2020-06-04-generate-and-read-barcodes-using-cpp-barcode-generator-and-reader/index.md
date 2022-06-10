---
title: 'Generate and Read Barcodes using C++'
seoTitle: "Generate and Read Barcode in C++ | C++ Barcode Generator and Reader"
description: "Generate barcode using C++. Scan and read barcodes including QR, Aztec, DataMatrix, Code128, and other barcodes in C++. C++ Barcode Generator and Reader."
date: Thu, 04 Jun 2020 05:49:06 +0000
draft: false
url: /2020/06/04/generate-and-read-barcodes-using-cpp-barcode-generator-and-reader/
author: Usman Aziz
summary: ''
tags: ['Cpp Barcode Generator and Reader', 'Generate and Read Barcode in Cpp']
categories: ['Aspose.BarCode Product Family']
---

In this article, I'll demonstrate how to **generate barcodes programmatically using C++**. You will also learn how to implement a **barcode scanner or reader** within your **C++** applications.



{{< figure align=center src="images/Generate-Barcode-in-C.jpg" alt="generate barcode in C++">}}


Barcodes are used to visually represent the data in the machine-readable form. The said technology has proved to be useful especially in the automated checkout systems deployed in stores and supermarkets. Almost every product in the market these days contains a barcode on it. This widespread popularity of the barcode has extended its use cases in various domains. Keeping an eye on the importance of barcodes, a few years ago, Aspose has launched barcode generator and reader API for various platforms. This article aims to showcase how to implement the barcode generator and reader within the C++ applications to dynamically generate and read barcodes.

*   [Generate a barcode using C++][1]
*   [Generate 2D barcode (QR or other) using C++][2]
*   [Create barcodes with a customized appearance using C++][3]
*   [Create barcodes with a caption using C++][4]
*   [Scan and read barcodes using C++][5]
*   [Read multiple barcode symbologies using C++][6]

## C++ Barcode Generator and Reader API

[Aspose.BarCode for C++][7] is a feature-rich C++ API for generating and reading a multitude of 1D and 2D barcodes. It lets you generate, customize, and export the barcodes to high-quality images. You can download the library files from the [Downloads][8] section. The downloadable package also contains a demo C++ application for you.

The following is the list of barcode symbologies you can generate using Aspose.BarCode for C++:

*   Code128
*   Code39 Standard
*   Code39 Extended
*   Code93 Standard
*   Code93 Extended
*   Code11
*   Codabar
*   BooklandEAN
*   EAN13
*   EAN8
*   EAN128
*   Interleaved2of5
*   Standard2of5
*   MSI
*   Postnet
*   Planet
*   UPCA
*   UPCE
*   EAN14(SCC14)
*   SSCC18
*   ITF14
*   BarCode supplement
*   Pdf417
*   QR
*   Datamatrix
*   Matrix 2 of 5
*   PZN (Pharma Zentral Nummer, Pharmazentralnummer barcode)
*   Deutsche Post Identcode
*   Aztec
*   Australia Post

## Generate a Barcode using C++ {#Generate-a-barcode-using-C++}

Generating a barcode using Aspose.BarCode can be achieved within a couple of lines of code. The following are the steps to perform this operation.

*   Create an object of the [BarcodeGenerator][9] class.
*   Initialize the object with the barcode's encode type and its text.
*   Generate barcode using [BarcodeGenerator->Save(System::String)][10] method.

The following code sample shows how to generate a barcode using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "generate-barcode.cpp" >}}

The following is the barcode we have generated using the above code.



{{< figure align=center src="images/code39_barcode-1024x298.jpg" alt="">}}


## Generate 2D Barcode (QR or other) using C++ {#Generate-2D-barcode-QR-or-other-using-C++}

In the previous example, we have created a one-dimensional barcode. Lets now create a two-dimensional barcode such as QR code. The following are the steps to create a QR barcode.

*   Create an object of the [BarcodeGenerator][11] class.
*   Initialize the object with the _EncodeTypes::QR_ type and set its text.
*   Create barcode image using [BarcodeGenerator->Save(System::String)][12] method.

The following code sample shows how to generate a QR barcode using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "generate-qr-barcode.cpp" >}}

The following QR code will be generated using the above code.



{{< figure align=center src="images/QR_Code.jpg" alt="">}}


## Generate Customized Barcodes using C++ {#Create-barcodes-with-a-customized-appearance-using-C++}

You can also customize the appearance of the barcode. For example, you can set the foreground color, background color, size, border style and etc. The following ate the steps to customize the barcodes using Aspose.BarCode for C++.

*   Create and initialize the object of the [BarcodeGenerator][13] class.
*   Access the barcode parameters using [BarcodeGenerator->get\_Parameters()][14] methods.
*   Set the desired parameters.
*   Generate the barcode and save it as an image.

The following code sample shows how to generate a customized barcode using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "generate-custom-barcode.cpp" >}}

The following is the customized Aztec barcode we have generated.



{{< figure align=center src="images/custom_barcode.jpg" alt="">}}


## Generate Barcodes with a Caption using C++ {#Create-barcodes-with-a-caption-using-C++}

Barcodes may also contain the caption below or above the barcode. You can set the caption's text as well as its visibility in the barcode image. The following code sample shows how to generate a barcode with the captions using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "generate-barcode-with-caption.cpp" >}}

The following is a barcode with the above and below captions.



{{< figure align=center src="images/barcode_caption-1024x319.jpg" alt="">}}


## Scan and Read Barcodes using C++ {#Scan-and-Read-Barcodes-using-C++}

Lets now see how to scan and read the barcodes using Aspose.BarCode for C++. The following are the steps to perform this feature.

*   Create an instance of the [BarCodeReader][15] class.
*   Initialize _BarCodeReader_ instance with the barcode's image file and it's symbology.
*   Use [BarCodeReader->Read()][16] method to retrive the text and type of the barcode.

The following code sample shows how to scan and read a barcode using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "read-barcode.cpp" >}}

## Read Barcodes with Multiple Symbologies using C++ {#Read-multiple-barcode-symbologies-using-C++}

Most of the time, an image contains only a single barcode symbology. However, in certain cases, the image may contain barcodes of multiple symbologies at the same time. In such cases, you can provide a list of the barcode symbologies to be scanned and read.

The following code sample shows how to scan an image having multiple barcode symbologies using C++.

{{< gist aspose-com-gists 281552f8ccf17e6b5ae4e313414184a8 "read-multiple-symbologies.cpp" >}}

## Conclusion

In this article, you have learned how to generate barcodes with different symbologies using C++. In addition, the procedure of scanning and reading barcodes is also discussed along with C++ code samples. You can explore more about the API using the [documentation][17].

## See Also

*   [Generate Barcodes using Java][18]
*   [Generate Barcodes using PHP][19]




[1]: #Generate-a-barcode-using-C++
[2]: #Generate-2D-barcode-QR-or-other-using-C++
[3]: #Create-barcodes-with-a-customized-appearance-using-C++
[4]: #Create-barcodes-with-a-caption-using-C++
[5]: #Scan-and-Read-Barcodes-using-C++
[6]: #Read-multiple-barcode-symbologies-using-C++
[7]: https://products.aspose.com/barcode/cpp
[8]: https://downloads.aspose.com/barcode/cpp
[9]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.generation.barcode_generator/
[10]: https://apireference.aspose.com/barcode/cpp/class/system.string/
[11]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.generation.barcode_generator/
[12]: https://apireference.aspose.com/barcode/cpp/class/system.string/
[13]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.generation.barcode_generator/
[14]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.generation.barcode_generator/#acd7573dd0e4e535164f5412f5d6d0548
[15]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.bar_code_recognition.bar_code_reader/
[16]: https://apireference.aspose.com/barcode/cpp/class/aspose.bar_code.bar_code_recognition.bar_code_reader#a5a37295fcf099a29ee5797beaedbfce0
[17]: https://docs.aspose.com/display/barcodecpp/Product+Overview
[18]: https://blog.aspose.com/2020/04/07/generate-or-scan-barcode-qr-pdf417-datamatrix-aztec-in-java/
[19]: https://blog.aspose.com/2020/01/29/php-barcode-generator-reader-and-scanner-api/





