---
title: 'Generate Barcode in Node.js Applications'
seoTitle: "Generate Barcode in Node.js | Generate Code128, Aztec, Pdf417, EAN etc"
description: "Use barcode generator API to generate barcodes in Node.js applications. Generate Code128, Aztec, Pdf417, EAN and variuos other barcodes in Node.js."
date: Thu, 06 May 2021 23:41:43 +0000
draft: false
url: /2021/05/06/generate-barcodes-in-node-js-applications/
author: Usman Aziz
summary: '[Barcodes][1] are used to visually represent the data in the form of graphical objects. Different types of barcodes are used in various cases, such as Code128, QR code, Aztech, Pdf127, and etc. In this article, you will learn how to implement barcode generation features in your web applications. Particularly, the article will cover **how to generate barcodes of different symbologies within Node.js applications**.'
tags: ['Generate a Barcode in Nodejs', 'Generate a QR Barcode in Nodejs', 'Nodejs Barcode Generator API']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/Generate-Barcode-in-Java-2.png" alt="generate barcode in node.js">}}


[Barcodes][2] are used to visually represent the data in the form of graphical objects. Different types of barcodes are used in various cases, such as Code128, QR code, Aztech, Pdf127, and etc. In this article, you will learn how to implement barcode generation features in your web applications. Particularly, the article will cover **how to generate barcodes in Node.js applications**.

*   [Node.js Barcode Generator API][3]
*   [Generate a Barcode in Node.js][4]
*   [Generate a QR Code in Node.js][5]
*   [Customize Appearance of a Barcode][6]

## Node.js Barcode Generator API {#Node.js-Barcode-Generator-API}

In order to generate barcodes, we will use [Aspose.BarCode for Node.js via Java][7]. It is a feature-rich API that lets you generate and read popular barcode symbologies from within your Node.js applications. You can either [download][8] the API or install it using the following NPM command.

```
> npm install aspose.barcode
```

Aspose.BarCode for Node.js via Java supports the following barcode symbologies.

<figure class="wp-block-table is-style-stripes"><table><tbody><tr><td>Australia Post</td><td>EAN8</td></tr><tr><td>Aztec</td><td>Interleaved2of5</td></tr><tr><td>BarCode supplement</td><td>ITF14</td></tr><tr><td>BooklandEAN</td><td>Matrix 2 of 5</td></tr><tr><td>Codabar</td><td>MSI</td></tr><tr><td>Code11</td><td>Pdf417</td></tr><tr><td>Code128</td><td>Planet</td></tr><tr><td>Code39 Extended</td><td>Postnet</td></tr><tr><td>Code39 Standard</td><td>PZN (Pharma Zentral Nummer, Pharmazentralnummer barcode)</td></tr><tr><td>Code93 Extended</td><td>QR</td></tr><tr><td>Code93 Standard</td><td>SSCC18</td></tr><tr><td>Datamatrix</td><td>Standard2of5</td></tr><tr><td>Deutsche Post Identcode</td><td>Swiss QR</td></tr><tr><td>EAN128</td><td>UPCA</td></tr><tr><td>EAN13</td><td>UPCE</td></tr><tr><td>EAN14(SCC14)</td><td></td></tr></tbody></table></figure>

## Generate a Barcode in Node.js {#Generate-a-Barcode-in-Node.js}

The following are the steps to generate a barcode in Node.js applications.

*   First, create an object of [BarcodeGenerator][9] class and set the barcode's type in its constructor, e.g. _EncodeTypes.CODE\_128_.
*   Set barcode's text using [BarcodeGenerator.setCodeText(string)][10] method.
*   Finally, generate the barcode's image using [BarcodeGenerator.save(string, string)][11] method.

The following code sample shows how to generate a barcode image in Node.js.

{{< gist aspose-com-gists 6fc020ff4becc4c21b8ee167210e8eb7 "generate-barcode.js" >}}

### Barcode



{{< figure align=center src="images/generate-barcode-java.png" alt="generate barcode node.js">}}


## Generate a QR Code in Node.js {#Generate-QR-Barcode-in-Node.js}

Aspose.BarCode for Node.js via Java also allows you to generate two-dimensional barcodes such as QR codes. The following are the steps to generate a QR code in Node.js.

*   First, create an object of [BarcodeGenerator][12] class and pass _EncodeTypes.QR_ to its constructor.
*   Set QR barcode's text using [BarcodeGenerator.setCodeText(string)][13] method.
*   Finally, generate QR code's image using [BarcodeGenerator.save(string, string)][14] method.

The following code sample shows how to generate a QR code in Node.js.

{{< gist aspose-com-gists 6fc020ff4becc4c21b8ee167210e8eb7 "generate-qr-barcode.js" >}}

### QR Code



{{< figure align=center src="images/generate-qr-barcode-java.png" alt="generate QR node.js">}}


## Customize Appearance of a Barcode {#Customize-Appearance-of-Barcode}

You can also customize the appearance of a barcode by changing the forecolor, back color, font, border, resolution, etc. The following are the steps to customize the appearance of a barcode.

*   First, create an object of [BarcodeGenerator][15] class and set the barcode's type in its constructor, e.g. _EncodeTypes.AZTEC_.
*   Set barcode's text using [BarcodeGenerator.setCodeText(string)][16] method.
*   Customize the barcode using its parameters, such as set back color using [BarcodeGenerator.getParameters().setBackColor("#A9A9A9")][17] method.
*   Finally, generate the barcode's image using [BarcodeGenerator.save(string, string)][18] method.

The following code sample shows how to customize a barcode in Node.js.

{{< gist aspose-com-gists 6fc020ff4becc4c21b8ee167210e8eb7 "generate-barcode-customize.js" >}}

### Barcode



{{< figure align=center src="images/generate-barcode-custom-appearance.png" alt="customize barcode">}}


## Get a Free API License

In order to use the API without evaluation limitations, you can [get a free temporary license][19].

## Conclusion

In this article, you have learned how to generate a barcode in Node.js applications. Also, you have seen how to customize the appearance of the barcodes using different options. Furthermore, you can explore more about the API using its [documentation][20]. In addition, you can share your queries with us via our [forum][21].

## See Also

*   [Read Barcodes using C# Barcode API][22]
*   [Scan Barcodes Programmatically using Java][23]




[1]: https://en.wikipedia.org/wiki/Barcode
[2]: https://en.wikipedia.org/wiki/Barcode
[3]: #Node.js-Barcode-Generator-API
[4]: #Generate-a-Barcode-in-Node.js
[5]: #Generate-QR-Barcode-in-Node.js
[6]: #Customize-Appearance-of-Barcode
[7]: https://products.aspose.com/barcode/nodejs-java
[8]: https://downloads.aspose.com/barcode/nodejs
[9]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator
[10]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#setCodeText
[11]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#save
[12]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator
[13]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#setCodeText
[14]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#save
[15]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator
[16]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#setCodeText
[17]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#getParameters
[18]: https://apireference.aspose.com/barcode/nodejs/BarcodeGenerator#save
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/barcode/nodejsjava/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/10/20/scan-and-read-barcodes-using-csharp/
[23]: https://blog.aspose.com/2020/04/07/generate-or-scan-barcodes-qr-codes-in-java-using-java-barcode-library/





