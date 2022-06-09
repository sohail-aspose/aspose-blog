---
title: 'PHP Barcode Generator and Reader API - Generate and Scan Barcodes in PHP'
seoTitle: ""
description: ""
date: Wed, 29 Jan 2020 17:54:19 +0000
draft: false
url: /2020/01/29/php-barcode-generator-reader-and-scanner-api/
author: Usman Aziz
summary: ''
tags: ['Aspose.BarCode for PHP via Java', 'barcode generator API in PHP', 'barcode scanner in php', 'php barcode generator', 'php barcode generator tutorial', 'php barcode reader', 'qr code generator and reader in php']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="PHP Barcode Generator Library">}}


**Barcodes** are used to visually represent the data about an object in the machine-readable form. It is more popular to keep the data about products which can be read using the **barcode scanners**. In order to make it possible to generate and read a variety of barcodes in the PHP based web applications, we have released [Aspose.BarCode for PHP via Java][1] - an easy to use **PHP barcode generator and reader API** which is designed to work via [Java Bridge][2].

In this article, I will present the recipes and code samples of how to **generate and read the barcodes using PHP** in your web applications. After reading this article, you'll be able to:

*   [generate a barcode using PHP barcode generator][3]
*   [generate 2D barcodes such as QR using PHP][4]
*   [create barcodes with a customized appearance in PHP][5]
*   [generate barcodes with a caption using PHP][6]
*   [scan and read a barcode using PHP barcode reader][7]
*   [scan and read a barcode with a particular symbology in PHP][8]

## PHP Barcode Generator and Reader - Installation and Usage

The installation of _Aspose.BarCode for PHP via Java_ consists of a few simple steps. The following are the pre-requisites of the API:

*   [PHP 7.0 or higher][9]
*   [Java SE Development Kit 1.7 or higher][10]
*   [Java Bridge][11]

You can [download][12] the complete package containing the API's JAR file, _Java Bridge.jar_, _Java.inc_, and ready to run source code examples to read, generate and recognize barcodes using PHP. In order to run the examples, following the below steps:

*   Run _JavaBridge_ server using _run-bridge.bat_ (available in the package).
*   Open _doc/examples/php\_side/how\_to\_generate\_barcode\_examples.php_ in the browser or run it using the command line.

## Generate Barcodes using PHP Barcode Generator {#generate-a-barcode-using-PHP-barcode-generator}

Once you have set up the environment, you can begin working with barcodes in your PHP based application. _Aspose.BarCode for PHP via Java_ supports a variety of barcode symbologies including:

*   Code128
*   Code11
*   Code39
*   QR
*   Datamatrix
*   EAN13
*   EAN8
*   ITF14
*   PDF417
*   and [many more][13].

The following is the simple recipe to generate a barcode of any supported symbology using PHP:

*   Create an object of _BarcodeGenerator_ class and initialized it with the desired encoding type and code text.
*   Generate barcode using _BarcodeGenerator->save()_ method.

The following code sample shows how to generate a barcode using PHP.

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-generator.php" >}}

### Output



{{< figure align=center src="images/generate-barcode.png" alt="PHP Barcode Generator">}}


## Generate 2D Barcodes using PHP Barcode Generator {#generate-2D-barcodes-such-as-QR-using-PHP}

Two-dimensional barcodes are represented as squares or the rectangles containing multiple dots. _Aspose.BarCode for PHP via Java_ also supports various 2D barcode types such as QR, PDF417, etc. The following code sample shows how to generate a QR barcode using PHP:

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-generator-QR.php" >}}

### Output



{{< figure align=center src="images/generate-QR-code.png" alt="QR Code Generator in PHP">}}


## Generate Barcodes with a Customized Appearance in PHP {#generate-barcodes-with-a-customized-appearance-in-PHP}

_Aspose.BarCode for PHP via Java_ also lets you customize the appearance of the barcodes. For example, you can set the background, foreground or border color of the barcode. The following code sample shows how to generate a barcode with a customized appearance in PHP.

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-generator-custom-appearance.php" >}}

### Output



{{< figure align=center src="images/generate-barcode-customize-apprearance-1024x209.png" alt="Generate Barcode in PHP">}}


## Generate Barcode with Caption in PHP {#Generate-Barcode-with-Caption-in-PHP}

You can also set as well as customize the appearance of the barcode's caption. The following code sample shows how to set the barcode's caption and customize its font.

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-generator-caption.php" >}}

### Output



{{< figure align=center src="images/generate-barcode-caption_png.png" alt="PHP Barcode Library ">}}


## Read a Barcode using PHP Barcode Reader {#scan-and-read-a-barcode-using-PHP-barcode-reader}

Along with the barcode generator, the API also provides you a powerful barcode reader to scan the barcodes and extract the data. The following is the recipe for how to read a barcode.

*   Create an instance of _BarcodeReader_ and initialize it with the file's path.
*   Read barcode using _BarcodeReader->read()_ method.
*   Get barcode type and text using _BarcodeReader->getCodeTypeName()_ and _BarcodeReader->getCodeText()_ methods.

The following code sample shows how to read a barcode using PHP.

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-reader.php" >}}

## Read Barcode with a Particular Symbology using PHP Barcode Reader {#scan-and-read-a-barcode-with-a-particular-symbology-in-PHP}

**Barcode Recognition** is the process of identifying the type of barcode we want to scan or read. In the previous example, we simply read a barcode without knowing its symbology type. However, in some cases, we know about the symbology of the barcode in advance. In such a scenario, we can speed up the scanning process by providing the barcode symbology explicitly to the barcode reader.

The following code sample shows how to read a barcode of a specific symbology using PHP.

{{< gist aspose-com-gists 87983edcfd83f707f41905abdd40ff67 "barcode-reader-specific-symbology.php" >}}

## Advanced Features of PHP Barcode Generator and Reader API

_Aspose.BarCode for PHP via Java_ provides a wide range of features for manipulating barcodes using PHP. You may have a look at the following documentation articles and simply port the Java code to PHP.

*   [2D Barcode Features][14]
*   [Set Height of Bars in Barcode][15]
*   [Use Checksum and Supplement Data for Barcodes][16]
*   [Generate a Patch Code][17]
*   [Working with Barcode Image][18]
*   [Optimize Barcode Scanning][19]
*   [Advanced Barcode Recognition Features][20]

In case you would find anything confusing or difficult for you, feel free to contact us via our [forum][21].

## See Also

*   [Generate and Scan Barcodes using Java][22]
*   [Generate Barcodes in Node.js Applications][23]




[1]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+PHP+via+Java+19.12
[2]: https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/exploded/JavaBridge.jar/download
[3]: #generate-a-barcode-using-PHP-barcode-generator
[4]: #generate-2D-barcodes-such-as-QR-using-PHP
[5]: #generate-barcodes-with-a-customized-appearance-in-PHP
[6]: #Generate-Barcode-with-Caption-in-PHP
[7]: #scan-and-read-a-barcode-using-PHP-barcode-reader
[8]: #scan-and-read-a-barcode-with-a-particular-symbology-in-PHP
[9]: https://www.php.net/downloads.php
[10]: https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html
[11]: https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/exploded/JavaBridge.jar/download
[12]: https://downloads.aspose.com/barcode/php
[13]: https://docs.aspose.com/display/barcodejava/Barcode+Supported+Symbologies
[14]: https://docs.aspose.com/display/barcodejava/Basic+2D+Barcode+Features
[15]: https://docs.aspose.com/display/barcodejava/Set+Height+of+the+Bars+in+the+Barcode+Image
[16]: https://docs.aspose.com/display/barcodejava/Use+Checksum+and+Supplement+Data+for+Barcodes
[17]: https://docs.aspose.com/display/barcodejava/How+to+Generate+a+Patch+Code
[18]: https://docs.aspose.com/display/barcodejava/Working+with+Barcode+Image
[19]: https://docs.aspose.com/display/barcodejava/Optimize+Scan
[20]: https://docs.aspose.com/display/barcodejava/Advanced+Barcode+Recognition+Features
[21]: https://forum.aspose.com/c/barcode
[22]: https://blog.aspose.com/2020/04/07/generate-or-scan-barcodes-qr-codes-in-java-using-java-barcode-library/
[23]: https://blog.aspose.com/2021/05/06/generate-barcodes-in-node-js-applications/





