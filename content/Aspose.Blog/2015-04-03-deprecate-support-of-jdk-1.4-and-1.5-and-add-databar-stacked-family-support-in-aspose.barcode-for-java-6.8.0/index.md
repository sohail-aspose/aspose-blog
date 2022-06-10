---
title: 'Deprecate Support of JDK 1.4 and 1.5 and Add DataBar Stacked Family Support in Aspose.BarCode for Java 6.8.0'
date: Fri, 03 Apr 2015 20:40:07 +0000
draft: false
url: /2015/04/03/deprecate-support-of-jdk-1.4-and-1.5-and-add-databar-stacked-family-support-in-aspose.barcode-for-java-6.8.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Total Product Family', 'Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)Good news for Aspose barcode community, we have released the new version of Aspose.BarCode for Java 6.8.0. This new release supports the DataBar Stacked, DataBar Expanded and DataBar Stacked Omnidirectional symbologies. Our users can now add encoding and decoding operations to their Java applications. DataBar stacked is a variation of the RSS-14 symbology that is stacked in two rows and is used when the normal symbol would be too wide for the application. This new release also supports encoding of Patch Code symbology, includes a new Line Codes Restoration filter, allows to check the license status.

## Deprecate the Support of JDK 1.4 and 1.5

Previously, we were providing two jar files. One for the JDK 1.4 and higher versions and other for the JDK 1.6 and higher versions. In this new release, we have dropped the support of JDK 1.4 and JDK 1.5. Since, we have provided a single jar for JDK 1.6 or higher versions. It is because both JDKs are discontinued by Sun/Oracle. Even commercial (non-open) support of JDK 1.5 is dropped about a year ago. **If you are presently using JDK 1.4.x or 1.5.x, you must upgrade your JDK prior to migrating to this new release.**

## DataBar Stacked, DataBar Expanded Stacked and DataBar Stacked Omnidirectional Symbologies

The sample code below specifies the use of Aspose.BarCode API.

*   **DataBar Stacked** is a variation of the RSS-14 symbology that is stacked in two rows and is used when the normal symbol would be too wide for the application.
*   **DataBar Expanded Stacked** barcode can grow vertically, it can encode a large amount of data in small space.
*   **DataBar Omnidirectional Stacked** is perfectly suitable for POS (point of sale) applications.

### DataBar Stacked Generation```
// Initialize BarCodeBuilder class object
BarCodeBuilder builder = new BarCodeBuilder();
// Set code text
builder.setCodeText("(01)00012345678905");
// Set symbology type
builder.setSymbologyType(Symbology.DatabarStacked);
// Save barcode image
builder.save("databarstacked.png");
```

Result:

[![][2]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/11/databarstacked1.png)

### DataBar Stacked Recognition```
// Define BarCodeReader class object
BarCodeReader reader;
// Initialize reader object
reader = new BarCodeReader("databarstacked.png", BarCodeReadType.DatabarStacked);

// Scan barcode image
if (reader.read())
{
    // Get code text
    System.out.println(reader.getCodeText());
}
// Dispose reader object
reader.close();
```

Result: (01)0001234567890

## Patch Code Encoding using Aspose.BarCode for Java

We've added encoding support of Patch code symbology, whereas decoding capability is already present. The Patch Codes aid in batch scanning of documents. It is a specific barcode and often is used in whole pages. Following help topic shows, how developers can generate whole page: How to Generate a Patch Code

## Line Codes Restoration Filter

We've added a new Line Codes Restoration filter. This filter restores corrupted strokes for 1D barcodes. This degradation could come from dirty, dusty products or discarded barcode resulting in touched or missing parts of the bars. For other details, please go through the help topic: Better and Faster Image Processing for Barcode Recognition

The major areas include enhancing of the barcode image,  improve accuracy of recognition, stop cropping of code text while change in resolution and improve recognition performance. This release comprises a number of key fixes that help us reading and writing capabilities.

*   Fixed: Cropped text after resolution changing.
    
*   Fixed: Incorrect GS1Code128 bar pattern/sequence
    
*   Fixed: Performance issue while reading PDF417 and Code128 codes
    
*   Fixed: Incorrect GS1Code128 bar sequence
    
*   Fixed: Can't generate a Databar Expanded code with a specified string
    
*   Fixed: String index out of range error message while generating a Code128 symbology
    
*   Fixed: InvalidOperationException while recognizing an Interleaved2of5 code
    
*   Fixed: Can't put two FNC1 characters in type GS1 DataMatrix
    
*   Fixed: Can't recognize PDF417 code from png image
    
*   Fixed: Can't recognize DataMatrix code from a tif file
    
*   Fixed: Can't read Code128 barcode from JPG image
    
*   Fixed: Can't recognize PDF417 barcode from the TIF image
    
*   Fixed: Can't read Code39 from the tif file
    
*   Fixed: Can't recognize QR code form the PDF document
    
*   Fixed: Can't recognize Code39 codes from the JPG file
    
*   Fixed: Unable to recognize the second EAN13 barcode from jpg image
    
*   Fixed: Can't recognize Code128 code from the TIF image
    
*   Fixed: code39 barcode not found from the scanned tif image
    
*   Fixed: Incorrect recognition of Code128 codes from a tif file
    
*   Fixed: Incorrect recognition of Code128 code from the jpg image
    
*   Fixed: Incorrection recognition of PDF417 code from the tif format
    
*   Fixed: Incorrect recognition of Pharmacode from the JPG image
    
*   Fixed: Incorrect type recognition of UPC and EAN barcodes
    
*   Fixed: Multiple incorrect recognitions of a single Pharmacode
    
*   Fixed: Incorrect recognition of a linear code from JPG image
    

## Aspose.BarCode for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][3]
    
*   [Download Aspose.BarCode for Java][4]
    
*   Aspose.BarCode for Java Wiki docs - help documentation and API reference documents.
    
*   [Aspose.BarCode Product Family Forum][5] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
    
*   [Enable Email Subscription][6] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
    
*   [Aspose.BarCode for Java Examples][7] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/11/databarstacked1.png "databarstacked"
[3]: http://www.aspose.com/java/barcode-component.aspx
[4]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx
[5]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/asposebarcode/Aspose_BarCode_JAVA




