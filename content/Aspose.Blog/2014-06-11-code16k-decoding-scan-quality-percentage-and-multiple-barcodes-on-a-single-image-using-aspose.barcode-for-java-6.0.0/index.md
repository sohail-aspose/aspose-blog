---
title: 'Code16K Decoding, Scan Quality Percentage and Multiple Barcodes on a Single Image using Aspose.BarCode for Java 6.0.0'
date: Wed, 11 Jun 2014 19:58:29 +0000
draft: false
url: /2014/06/11/code16k-decoding-scan-quality-percentage-and-multiple-barcodes-on-a-single-image-using-aspose.barcode-for-java-6.0.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)Good news for our barcode community, we have released the new build of Aspose.BarCode for Java 6.0.0. This new release addresses the performance, time and memory consumption issues, and brings overdue updates to resolve issues reported in the Aspose forums. Also, some advanced new features are added. These features allow developers to let their end users be more self-sufficient.

## Decode Code16K Symbology

There are many different types of barcodes, often referred to as barcode symbologies. From this release, the Aspose.BarCode API enables developers to decode the Code16K symbology. In the previous version, we added Code16K encoding; now both encoding and decoding Code16K are supported.

## Get all Possible 1D Barcodes from an Image

Users can now retrieve all possible 1D barcodes using a single method call. The BarCodeReader.getAllPossibleBarCodes method allows them to do so. Please find the details of this feature in the following help topic: Get all Possible 1D Barcodes from an Image.

## Get BarCode Recognition Quality in Percent

Barcode recognition percentage gives a clear picture based on the quality and performance parameters. The BarCodeReader.getRecognitionQuality method helps with that. You can find the details of this feature in the following help topic: Get BarCode Recognition Quality in Percent.

## Performance, Time and Memory Improvements

We noticed time and memory consumption problems with the PatchCode symbology. When scanning PatchCodes from TIFF files memory consumption was around 150MB to 200MB. This has is now been fixed and memory usage is now around 40MB. Also, these sample graphics now take only 1.6 seconds to be recognized.

The DataMatrix performance with large pictures has been upgraded. Previously, it took too long to be recognized. Key factors of this improvement are “Diagonal check” and “Strict angle check”.

## Generate Multiple Barcodes on a Single Image

It's now easy to generate multiple barcodes on a single image. We just need to follow a simple code snippet. You can find the details of this feature in the following help topic: Generate Multiple Barcodes on a Single Image.

## Throw Exception when Code Text is Incorrect (1D Barcodes)

The BarCodeBuilder.setThrowExceptionWhenCodeTextIncorrect method has been added for 1D barcodes. If the code text is incorrect and the value is set to true, an exception is thrown; else, the code text is corrected to match the barcode’s specification. An exception is always thrown for Databar symbologies if the code text is incorrect. It is never thrown for AustraliaPost, SingapurePost, Code39Extended, Code93Extended, Code16K, and Code128 symbologies if codetext is incorrect. Please see the following topic for help: 1D Barcodes with Optional Exception Message in Case of Wrong Code Text.

## Public API Changes

The following API changes in the new version are worth noting:

*   The BarCodeBuilder.saveAsEmf(java.io.OutputStream) and saveAsEmf(java.lang.String) methods have been removed. The functionality was not implemented in earlier barcode versions and the both methods have been removed now since earlier methods threw the exception NotImplementedException.
    
*   The Code128CodeBuilder and Code128CodeSet classes have been removed. Now all codesets set and switched automatically according to code 128 specification. No need for code 128 builder to be public anymore. Additionally, all references to this class have been removed too: IBarCodeControl.getCode128CodeSet(), IBarCodeControl.setCode128CodeSet(Code128CodeSet), BarCodeBuilder.getCode128CodeSet(), BarCodeBuilder.setCode128CodeSet(int).
    
*   The BinarizedBitmap class has been removed. This class was obsolete and is not useful anymore. Since we have refactored the BarCode engine there is no need to use it directly and this class has been removed from the public API. Additionally, all the methods expecting BinarizedBitmap have been removed from the public API.
    
*   The field RecognitionHints.ImageBinarization.HLS has been removed. We have greatly refactored the BarCode engine and now we have found that HLS filters work the same way as GrayNormalization filter do. Previously HLS filter has been used for binarization but currently we use some other binarization algorithms. The following code:
    
    **Java**
    
    ```
    BarCodeReader reader = new BarCodeReader(image, BarCodeReadType.Code39Standard);
    reader.setImageBinarizationHints(RecognitionHints.ImageBinarization.HLS); 
    ```
    
    May be safely refactored to this with the new BarCode engine:
    
    **Java**
    
    ```
    BarCodeReader reader = new BarCodeReader(image, BarCodeReadType.Code39Standard);
    ```

## Bug Fixes and Improvements

The following fixes in the new version are also worth noting:

*   We have increased the minimum width of 1D barcodes.  Previously, we were getting different images than usual. The problem occurred during customizing the barcode width using lower values.
    
*   This new release also enhances PDF417 barcode encoding in compaction mode and includes all carriage returns.
    
*   The Code128 encoding has improved the presence of FNC characters. Previously, it generated incorrect code when a few FNC characters were present.
    
*   The Code128CodeBuilder class has been removed. It was used to generate customized code text for Code128 barcodes. We have updated the Code128 encoder to auto-handle this functionality.
    
*   The quality of the RM4SCC barcode processing, code text appearance and exception handling of the Pharmacodes symbology’s exceeding text is much better compared to the previous version.
    

Many other important fixes are done to improve the overall quality. These improvement areas include the accurate reading of the DataMatrix from PDF, Code128 from PDF, PDF417 from JPG and recognition failure of QR, PDF417, Code128 codes from graphics. Another performance improvement area is the barcode recognition on 64 bit operating system architecture. Barcode recognition was slower with 64 bit operating systems.

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




