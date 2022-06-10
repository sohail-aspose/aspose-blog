---
title: 'Code16K Decoding, Optimized Recognition Speed, Improved Quality and Performance in Aspose.BarCode for .NET 5.9.0.0'
date: Fri, 29 Nov 2013 07:18:37 +0000
draft: false
url: /2013/11/29/code16k-decoding-optimized-recognition-speed-improved-quality-and-performance-in-aspose.barcode-for-.net-5.9.0.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png)We are pleased to announce the release of Aspose.BarCode for .NET 5.9.0. With this release, the overall barcode recognition quality and performance have been greatly improved. These improvements have been made for different symbologies, image formats and 64bit operating systems. The overall performance improvement in this latest version is about 3 times the previous version.

The Code16K symbology is supported from this version. Many other significant enhancements have been made to improve the overall quality of RM4SCC, PatchCode, Pdf417, DataMatrix, QR and Pharmacode symbologies. The quality and performance have been enhanced for recognizing Patch Code and InterLeaved2of5 barcodes from TIFF images. The quality of PDF417 and QR codes recognition from JPG images has been improved as well. Similarly, the quality of DataMatrix code recognition from PDF files has been enhanced.

Another performance improvement area is the barcode recognition on 64bit operating system architecture. In addition to this the quality of the RM4SCC barcode processing, code text appearance and exception handling of Pharmacodes symbology’s exceeding text is much better compared to the previous version.

With this new version, you can also get all 1D barcodes using a single method. The BarCodeReader class' GetAllPossibleBarCodes method allows you to do that. You can find the details of this feature in the following help topic: Get all Possible 1D Barcodes from an Image.

The following changes in the new version are also worth noting:

*   The BarCodeBuilder.ThrowExceptionWhenCodeTextIncorrect property is only used for 1D barcodes. If the code text is incorrect and the value is set to true, an exception is thrown; else, the code text is corrected to match the barcode's specification. An exception is always thrown for Databar symbologies if the code text is incorrect. It is never thrown for AustraliaPost, SingapurePost, Code39Extended, Code93Extended, Code16K, and Code128 symbologies if codetext is incorrect. Please see the following topic for help: 1D Barcodes with Optional Exception Message in Case of Wrong Code Text.
    
*   The Code128CodeSet class has been removed. It allowed you to encode with different codesets whereas you do not need to worry about it anymore as it is now handled internally.
    
*   The Code128CodeBuilder class has been removed. It was used to generate customized code text for Code128 barcodes. We have updated the Code128 encoder to auto-handles all of this functionality.
    
*   The BinarizedBitmap class has been removed. There is no replacement for BinarizedBitmap because inside it is only a byte array, nothing more. Its code is the same with Bitmap class processing.
    

The Aspose.BarCode for .NET team has listened to all the suggestions shared by our customers and reviewed various scenarios in which customers use this product, and improved the product to provide best possible performance and quality. We’ll be looking forward to your feedback on this improved version.

To view a complete list of new features, fixes and enhancements [download the new release of Aspose.BarCode for .NET][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx




