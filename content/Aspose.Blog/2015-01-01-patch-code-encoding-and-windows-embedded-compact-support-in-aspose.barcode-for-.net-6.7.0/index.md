---
title: 'Work with Patch Code Encoding and Windows Embedded Compact using C#'
date: Thu, 01 Jan 2015 16:09:32 +0000
draft: false
url: /2015/01/01/patch-code-encoding-and-windows-embedded-compact-support-in-aspose.barcode-for-.net-6.7.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for .NET][1] 6.7.0. This new release supports encoding of Patch Code symbology, includes a new Line Codes Restoration filter, allows to check the license status  and improves Windows Embedded Compact support. We have also fixed several other defects.

## Patch Code Generation using C#

We've added encoding support of Patch code symbology, whereas decoding capability is already present. The Patch Codes aid in batch scanning of documents. It is a specific barcode and often is used in whole pages. Following help topic shows, how developers can generate whole page: [How to Generate a Patch Code][2]

## Support of Windows Embedded Compact

Aspose.BarCode for .NET API gives control to Windows Embedded Compact users to add barcode generation and recognition functionality in their .NET applications. Below is an Aspose.BarCode API code sample that shows how to use it.

### For Generation```
// set license file name
string licensefilename = "Aspose.BarCode.lic";
// initialize license class object
License license = new License();
// apply license
license.SetLicense(licensefilename);

// initialize BarCodeBuilder class object
BarCodeBuilder builder = new BarCodeBuilder(textBox1.Text, Symbology.DatabarStackedOmniDirectional);

// set dimensions
builder.xDimension = 2;
builder.yDimension = 4;

// display barcode picture
pictureBox1.Image = builder.BarCodeImage;
```

### For Recognition```
// set license file name
string licensefilename = "Aspose.BarCode.lic";
// initialize license class object
License license = new License();
// apply license
license.SetLicense(licensefilename);

// initialize BarCodeReader class object
BarCodeReader reader = new BarCodeReader((Bitmap)pictureBox1.Image,
BarCodeReadType.DatabarStackedOmniDirectional);
// scan image
reader.Read();
// get code text
textBox2.Text = reader.GetCodeText();
reader.Close();
```

Result: (01)0003456789012

## Line Codes Restoration Filter

We've added a new Line Codes Restoration filter. This filter restores corrupted strokes for 1D barcodes. This degradation could come from dirty, dusty products or discarded barcode resulting in touched or missing parts of the bars. For other details, please go through the help topic: [Better and Faster Image Processing for Barcode Recognition][3]

## Check License Status

We have added IsLicensed property in the License class. It helps to check the current status of the License that whether it is applied or not. In this regard, please see this help topic: [Check License Status of Aspose.BarCode for .NET][4]

This release comprises a number of key fixes that help us improve accuracy, less error messages and performance.

*   Fixed: Code39 barcode was not found from the scanned tif image.
*   Fixed: Can't recognize second EAN13 barcode from a JPG image.
*   Fixed: Can't generate a Databar Expanded code with a specified string.
*   Fixed: Can't recognize Code39 codes from the JPG file.
*   Fixed: Incorrect recognition of a linear code of JPG image.
*   Fixed: GS1 encoding and decoding logic for nonstandard variants.
*   Fixed: Performance issue while reading PDF417 and Code128 codes.
*   Fixed: Incorrect recognition of Code128 code of the JPG image.
*   Fixed: Can't recognize QR code from the PDF document.
*   Fixed: Can't read Code39 from the tif file.
*   Fixed: InvalidOperationException while recognizing an Interleaved2of5 code.

To view a complete list of API features and try the API, please visit the following page and [download the latest version of Aspose.BarCode for .NET][5]. If you need any help, please feel free to ask in the [Aspose.BarCode forum][6]. For more details, please visit the [Aspose.BarCode for .NET documentation][7].



[1]: https://products.aspose.com/barcode/net
[2]: https://docs.aspose.com/barcode/net/how-to-generate-a-patch-code/
[3]: https://docs.aspose.com/barcode/net/improve-barcode-recognition/#better-and-faster-image-processing-for-barcode-recognition
[4]: https://docs.aspose.com/barcode/net/licensing/
[5]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[7]: https://docs.aspose.com/barcode/net/




