---
title: 'Recognize BarCodes using new Decode Types in Java'
date: Tue, 11 Dec 2018 20:08:25 +0000
draft: false
url: /2018/12/11/recognize-barcodes-using-new-decode-types-in-aspose.barcode-for-java/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.BarCode for Java 18.11][1]. This release added new Decode Types in the API for better recognition of Barcodes. Enums names have also been changed to bring them in line with Java naming conventions. For a detailed note on what is new and fixed, please visit the [release notes][2] page of API documentation.

## New Decode Types to Recognize Barcode using Java

The new release of Aspose.Barcode provides additional Decode types that enhance the performance and ease of reading barcodes. You may use the newly added Decode types as shown below.

```
BarCodeReader reader = new BarCodeReader(folder + "Code11.png", 
DecodeType.TYPES_1D);
while (reader.read())
{
 String codeType = reader.getCodeType().toString();
 String codeText = reader.getCodeText();
 System.out.println(codeType + ", " + codeText);
}
result: Code11, 012345
 
BarCodeReader reader = new BarCodeReader(folder + "Postnet.png", 
DecodeType.POSTAL_TYPES);
while (reader.read())
{
 String codeType = reader.getCodeType().toString();
 String codeText = reader.getCodeText();
 System.out.println(codeType + ", " + codeText);
}
result: Postnet, 012345
 
BarCodeReader reader = new BarCodeReader(folder + "GS1Code128", 
DecodeType.MOST_COMMON_TYPES);
while (reader.read())
{
 String codeType = reader.getCodeType().toString();
 String codeText = reader.getCodeText();
 System.out.println(codeType + ", " + codeText);
}
result : GS1Code128, 012345
```

## Other Enhancements

Other than the addition of decode types, there are a number of other enhancements made to the API in this release. These enhancements are listed below:

*   Enum names have been renamed to match Java naming conventions.
*   Barcode reader has been enhanced with improved detection of the following barcodes
    *   3D-distorted barcodes
    *   2D-rotated barcodes
    *   CODE39 barcodes
*   GS1 DataBar Expanded Stacked barcode passes the GS1 Canada barcode verification.
*   You can now constrain the region for barcode detection to improve performance.
*   Enhanced MicrE13B for safe bitmap access.
*   Generate Databar Extended Stacked Barcode with 7 rows.
*   Implemented license setting with Open JDK 11
*   Improved API performance.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java][3]
*   [Download Aspose.BarCode for Java][4] – Install Aspose.BarCode for Java from Maven
*   [Aspose.BarCode for Java Wiki docs][5] – help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/18.11
[2]: https://docs.aspose.com/barcode/java/aspose-barcode-for-java-18-11-release-notes/
[3]: https://products.aspose.com/barcode/java
[4]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-barcode/
[5]: https://docs.aspose.com/barcode/java/
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[8]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java




