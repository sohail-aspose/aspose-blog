---
title: 'New Image Processing Techniques, Code16K Encoding and SHA-2 Support in Aspose.BarCode for Java 5.8.0'
date: Wed, 19 Feb 2014 19:47:35 +0000
draft: false
url: /2014/02/19/new-image-processing-techniques-code16k-encoding-and-sha-2-support-using-aspose.barcode-for-java-5.8.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)Today we’re very pleased to announce the release of  Aspose.BarCode for Java 5.8.0. This version sees the barcode detection rate with dark or severely noised  images improved. You can also generate a barcode of Code16K symbology.

We have defined a few more rules regarding AustralianPosteParcel symbology. The API will throw an exception message when generating AustralianPosteParcel barcode with incorrect code text. If the code text is incorrect in recognition, a Code128 will be returned. Similarly, from now onward the BarCodeReader class' GetChecksum method returns a checksum for the RM4SCC symbology.

This month's release includes the ability to retrieve product name, assembly version, file version, release date, etc. You can find the details of this feature in the following help topic: Get the Product Name and Assembly Version Information.

The following fixes in the new version are also worth noting:

*   IBarCodeControl interface has been added. Implement this interface if you want to control how Aspose.BarCode builds barcode images.
    
*   CodabarSymbol enumeration has been added. The alphabet characters A, B, C, D are used to mark the beginning and end of the Codabar barcode. You can find the details in the following help topic: Set Start and Stop Symbols of Codabar Barcode
    
*   EnableChecksum enumeration has been added. Please find details in the following help article: Use Checksum and Supplement Data for Barcodes
    
*   RenderFormat enum has been added. It represents the image formats, rendering to the target.
    

## Value-added Image Processing Techniques

In order to improve the effectiveness of Aspose.BarCode, we have added two more image processing filters. Color quantification is the key factor.

*   **Complex background** technique can locate a barcode region in a complex or colored background through region-based image analysis.
    
*   **Invert image technique** inverts the image before recognition. It helps the code recognize images with a black background and white, or near white, barcode.
    

In addition to this, MedianSmoothingWindowSize gets or sets the median smoothing window size. Typical values are 3 or 4. The default value is 3. The recognition hint MedianSmoothing must be set. For noisy images, 4 is good value. You can find a complete example description in the following help topic: Better and Faster Image Processing for Barcode Recognition

## Sign JARs with SHA-2 Certificate

Secure Hash Algorithm (SHA-2) is now supported. Please note that some older applications and operating systems do not support SHA-2, for example, Windows™ XP Service Pack 2 or lower does not support the use of SHA-2. Java SDK 1.4.2 or higher needs to be installed and used on the server for SHA-2 support for Java server support.

## Real-time Upgraded Quality and Performance

This new release also adds strength to the whole barcode recognition quality and performance via advanced scanning  algorithms. We have incorporated a few fixes specifically for Code128, DataMatrix, Code39 and Aztec symbologies so far it could impact a bit more on these symbologies.

There are several other error message fixes when loading Code128 and Code93 codes or reading PDF417, DataMatrix and QR codes. These fixes can also lead to the quality and performance.

Many other important fixes are done to improve the overall quality. These improvement areas include the graphics loading time of Pdf417 and GS1Code128 codes, recognition failure of QR, Datamatrix, NonStandard DataMatrix, Code128, PDF417 and Code11, visibility of code text on EAN8, EAN13, UPCA and UPCE symbologies, incorrect recognition of the Datamatrix, Pdf417 codes, incomplete code text recognition of RM4SCC code, incorrect angle detection of Code39Extended code and wrong location when reading PostNet code.

To view a complete list of new features, fixes and enhancements [download the new release of Aspose.BarCode for Java][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx




