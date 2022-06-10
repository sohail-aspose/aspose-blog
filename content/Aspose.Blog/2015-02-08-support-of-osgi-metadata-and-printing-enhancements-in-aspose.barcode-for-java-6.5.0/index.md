---
title: 'Support of OSGi Metadata and Printing Enhancements in Aspose.BarCode for Java 6.5.0'
date: Sun, 08 Feb 2015 16:17:49 +0000
draft: false
url: /2015/02/08/support-of-osgi-metadata-and-printing-enhancements-in-aspose.barcode-for-java-6.5.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)Good news for our barcode community, we have released the new build of Aspose.BarCode for Java 6.5.0. This new release has added support of OSGi metadata to Aspose.BarCode for Java jars. The OSGi metadata enables jars to be used in the OSGi modular environment and be an OSGi Bundle. It also addresses the recognition performance, time and memory consumption issues, and brings overdue updates to resolve issues reported in the Aspose forums.

## BarCode Image Printing Improvements

Aspose.BarCode for Java 6.5.0 has exposed two new methods for the printing of barcode image.  In this regard, BarCodeBuilder.setPrinterName method allows to set the output printing source by accepting a string parameter and BarCodeBuilder.print method gives printing command to the printer. We had missed this feature support in the last few releases. It was due to the new modification to the code base. For details, please see this help topic: Printing a BarCode Image

**Java**

```
// Create instance of BarCodeBuilder, specify codetext and symbology in the constructor
BarCodeBuilder builder = new BarCodeBuilder("12345678", Symbology.Code128);
// Set printer name
builder.setPrinterName("ML-1640 Series");
// start print job
builder.print(); 
```

## BarCode Text Placements on the Image

Previously, users were facing issues in the code text alignment and 2D text display feature was not working properly. In this new version, we have managed to fix such issues. Now, the code text caption alignment settings and BarCodeBuilder.Display2DText method work properly.  This is the list of fixed issues:

*   Fixed: The code text of the bar code is not in the middle.
    
*   Fixed: Location of above caption was not correct for AZTEC barcode.
    
*   Fixed: builder.getCaptionBelow().setTextAlign method does not work as expected.
    
*   Fixed: BarcodeBuilder.Display2DText does not work in Java.
    

## Reading BarCodes and High Performance

Our development team is working hard to improve the reading capability, scanning performance and accurate detection of the several barcode types. In last few releases, we have added a remarkable progress. This release comprises a number of key fixes that help us improve decoding:

*   Fixed: Recognition performance issue with Code128 barcode.
    
*   Fixed: Unable to recognize Code128 symbol.
    
*   Fixed: Recognize GS1 Databar barcodes.
    
*   Fixed: Code93 recognition problem.
    
*   Fixed: Code128 Barcode is not recognized in jpg image.
    
*   Fixed: Code39 symbology is not recognized in tif image.
    
*   Fixed: BarCodeRecognition Orientation Test: 3 symbols got recognized from a total of 6.
    
*   Fixed: Unable to scan barcodes from a multipage tiff.
    
*   Fixed: Default resolution does not change when creating barcodes.
    
*   Fixed: code39 image recognition issue
    
*   Fixed: Test PDF417 image (PkDecode.jpg)
    

## Aspose.BarCode for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][2]
    
*   [Download Aspose.BarCode for Java][3]
    
*   Aspose.BarCode for Java Wiki docs - help documentation and API reference documents.
    
*   [Aspose.BarCode Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
    
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
    
*   [Aspose.BarCode for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: http://www.aspose.com/java/barcode-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposebarcode/Aspose_BarCode_JAVA




