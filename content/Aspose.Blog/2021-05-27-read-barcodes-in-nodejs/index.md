---
title: 'Read Barcodes in Node.js Applications'
seoTitle: "Read Barcodes in Node.js | Barcode Reader for Node.js | Aspose.BarCode"
description: "Use Node.js barcode API to read barcodes from within your Node.js applications. Recognize Code128, QR code, Aztec, Datamatrix, and other barcodes."
date: Thu, 27 May 2021 12:16:22 +0000
draft: false
url: /2021/05/27/read-barcodes-in-nodejs/
author: Usman Aziz
summary: 'Barcodes have become an essential part of the purchase process of the products. In a barcode, the information is represented as a one or two-dimensional graphical object. These graphical objects are recognized to read the encoded information. In order to automate barcode recognition, this article covers **how to read barcodes in Node.js applications**.'
tags: ['Barcode recognition in nodejs', 'Nodejs Barcode API', 'Read Barcodes in Nodejs', 'Read a Specific Barcode in nodejs']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/scan-and-read-barcodes-using-nodejs.jpg" alt="read barcode in nodejs">}}


Barcodes have become an essential part of the purchase process of the products. In a barcode, the information is represented as a one or two-dimensional graphical object. These graphical objects are recognized to read the encoded information. In order to automate barcode recognition, this article covers **how to read barcodes in Node.js using barcode reader API**.

*   [Node.js Barcode Reader API][1]
*   [Read Barcodes in Node.js][2]
*   [Read a Specific Barcode Type from an Image][3]
*   [Switch Barcode Recognition Modes][4]

## Node.js Barcode Reader API {#Nodejs-Barcode-API}

In order to read the barcodes from within the Node.js applications, we'll use [Aspose.BarCode for Node.js via Java][5]. It is a feature-rich API that lets you generate, scan, and read a wide range of barcode symbologies. You can either [download][6] the API's package or install it using the following NPM command.

```
> npm install aspose.barcode
```

## Read Barcodes in Node.js {#Read-Barcodes-in-Nodejs}

The following are the steps to read barcodes from an image in Node.js.

*   Create an object of [BarCodeReader][7] class and initialize it with the barcode image file.
*   Use [BarCodeReader.readBarCodes()][8] method to read the barcodes' text and type name.

The following code sample shows how to read barcodes in Node.js.

{{< gist aspose-com-gists cb6ddb3cf026a54b122d94f127c8dfbf "read-barcodes.js" >}}

## Read a Specific Barcode Type in Node.js {#Read-a-Specific-Barcode-in-an-Image}

You can also specify the type of barcode you want to read from the given image. As an example, the following are the steps to read a Code128 barcode.

*   First, create an object of [BarCodeReader][9] class and initialize it with the barcode image and type.
*   Use [BarCodeReader.readBarCodes()][10] method to read the barcodes' text and type name.

The following code sample shows how to read a specific barcode in Node.js.

{{< gist aspose-com-gists cb6ddb3cf026a54b122d94f127c8dfbf "read-particular-barcode.js" >}}

## Switch Barcode Recognition Modes {#Switch-Barcode-Recognition-Modes}

You can also switch the barcode recognition modes in order to tune the processing speed and quality as required. The following quality settings are supported by the API at the moment.

*   **Hight Performance**: To recognize high-quality barcodes.
*   **Hight Quality**: For low-quality barcodes.
*   **Max Barcodes**: To recognize all possible barcodes, even incorrect barcodes.
*   **Normal Quality**: Suitable for most of the barcodes.

The following are the steps to specify quality settings in barcode recognition process.

*   First, load the barcode image using [BarCodeReader][11] class and specify the type of barcode.
*   Set barcode recognition settings using [BarCodeReader.setQualitySettings()][12] method.
*   Finally, use [BarCodeReader.readBarCodes()][13] method to read the barcodes' text and type name.

The following code sample shows how to specify quality settings in barcode recognition in Node.js.

{{< gist aspose-com-gists cb6ddb3cf026a54b122d94f127c8dfbf "set-quality.js" >}}

## Get a Free API License

In order to use the API without evaluation limitations, you can [get a free temporary license][14].

## Conclusion

In this article, you have learned how to read barcodes in Node.js applications using barcode reader API. Furthermore, you have seen how to read barcodes with different quality settings. You can explore more about the API using its [documentation][15] and code samples available in the downloadable [package][16]. In addition, you can share your queries with us via our [forum][17].

## See Also

*   [Generate Barcodes in Node.js Applications][18]




[1]: #Nodejs-Barcode-API
[2]: #Read-Barcodes-in-Nodejs
[3]: #Read-a-Specific-Barcode-in-an-Image
[4]: #Switch-Barcode-Recognition-Modes
[5]: https://products.aspose.com/barcode/nodejs-java
[6]: https://downloads.aspose.com/barcode/nodejs
[7]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader
[8]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader#readBarCodes
[9]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader
[10]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader#readBarCodes
[11]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader
[12]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader#setQualitySettings
[13]: https://apireference.aspose.com/barcode/nodejs/BarCodeReader#readBarCodes
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/barcode/nodejsjava/
[16]: https://downloads.aspose.com/barcode/nodejs
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/05/06/generate-barcodes-in-node-js-applications/





