---
title: 'Generate or read Code32 and Datalogic2of5 barcodes and read MICR barcodes in Java'
date: Tue, 21 Jun 2016 07:33:23 +0000
draft: false
url: /2016/06/21/generate-or-read-code32-and-datalogic2of5-barcodes-and-read-micr-barcodes-in-java/
author: Muhammad Ijaz
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)We are pleased to announce the release of Aspose.BarCode for Java 7.8.0. This release supports generating Code32 and Datalogic2of5 barcodes. You can also read Code32, Datalogic and MICR barcodes. A new manual hint to skip rotated barcodes when reading barcode images has also been added to this release.

## Use manual hints to skip rotated barcodes

Aspose.Barcode for Java allows you to turns off the rotation algorithms and increases the recognition speed. BarCodeReader.setManualHints can be set to ManualHint.SkipRotatedBarcodes for this purpose e.g.

```
 long s = System.currentTimeMillis();
String filename = folder + "/Datamatrix12.jpg";

BarCodeReader reader = new BarCodeReader(filename, BarCodeReadType.GS1DataMatrix);
System.out.println("Skip rotated barcodes");
reader.setRecognitionMode(RecognitionMode.ManualHints);
reader.setManualHints(ManualHint.SkipRotatedBarcodes);

while (reader.read())
{
   System.out.println(reader.getReadType() + ": " + reader.getCodeText() + " QA:" + reader.getRecognitionQuality());
}
long res1 = System.currentTimeMillis() - s;
System.out.println(res1);
System.out.println();

s = System.currentTimeMillis();
reader = new BarCodeReader(filename, BarCodeReadType.GS1DataMatrix);
System.out.println("Not skip rotated barcodes");


while (reader.read())
{
    System.out.println(reader.getReadType() + ": " + reader.getCodeText() + " QA:" + reader.getRecognitionQuality());
}
long res2 = System.currentTimeMillis() - s;
System.out.println(res2); 
```

**Note**: It is available for Datamatrix and the linear barcodes only.

## Enhancements

Following is a list of improvements included in this release.

*   PDF417 barcode  recognition has been improved
*   Path IV barcode recognition has been improved
*   DataMatrix barcode recognition has been improved
*   More than 64 barcode types are supported
*   Aztec barcode recognition has been improved

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for Java 7.8.0 page in downloads section][2].

## Aspose.BarCode for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][3]
*   [Download Aspose.BarCode for Java][4]
*   Aspose.BarCode for Java Wiki docs – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][6] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: http://www.aspose.com/downloads/barcode/java
[3]: http://www.aspose.com/products/barcode/java
[4]: http://www.aspose.com/downloads/barcode/java
[5]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




