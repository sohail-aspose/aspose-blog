---
title: 'Read Barcode from Specified Area of Image using Java'
date: Fri, 25 Feb 2011 22:06:36 +0000
draft: false
url: /2011/02/25/read-barcode-from-specified-area-of-image-with-aspose.barcode-for-java/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We have recently released a new version of Aspose.BarCode for Java v2.5.1. With this version, you can now specify the area inside an image for reading barcodes. This feature is very useful for improving the performance in those cases where the image size is very large and the location of barcode is known in advance. The barcode reader will only scan the specified part instead of scanning the whole image.

Sample Java code:

```
// Get the image
Image img = Toolkit.getDefaultToolkit().getImage(“c:\\barcode.jpg”);
// New instance of BinarizedBitmap in which scan area is specified
BinarizedBitmap bBmp = new BinarizedBitmap(img, new Rectangle(0, 0, 672, 96));
// Scan the barcode inside the specified area only
BarCodeReader reader = new BarCodeReader(bBmp, BarCodeReadType.Code39Standard);
while (reader.read())
{
System.out.println(“codetext: ” + reader.getCodeText());
}
// Close the reader
reader.close();
```

It also includes other new features for generating the fixed size barcode image.

For release notes and download, please visit [https://products.aspose.com/barcode/java][1]




[1]: https://products.aspose.com/barcode/java




