---
title: 'New Decode Types and Renamed Enums in Aspose.BarCode for JasperReports'
date: Tue, 11 Dec 2018 20:49:58 +0000
draft: false
url: /2018/12/11/use-new-decode-types-and-renamed-enums-in-aspose.barcode-for-jasperreports/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-JasperReports_100.png" alt="Aspose.BarCode for JasperReports">}}


We are pleased to announce the release of [Aspose.BarCode for JasperReports][1] 18.11. This release added new Decode Types in the API for better recognition of Barcodes. Enums names have also been changed to bring them in line with Java naming conventions.  
To view a complete list of fixes, please visit [Aspose.Barcode for JasperReport 18.11 release notes][2] page.

## New subsets added to DecodeType

The new release of Aspose.Barcode provides additional Decode types which enhance the performance and ease of reading barcodes. You may use the newly added Decode types as shown below.

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

You can download the latest release of Aspose.BarCode for JasperReports from the following link:  
[Download Aspose.BarCode for JasperReports 18.11.][3]

## Aspose.BarCode for JasperReports Resources

The following API resources can be of help to you in getting started:

*   [Homepage for Aspose.BarCode for JasperReports API][4]
    
*   [Download Aspose.BarCode for JasperReports][5]
*   [Aspose.BarCode for JasperReports Wiki docs][6] - help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://products.aspose.com/barcode/jasperreports
[2]: https://docs.aspose.com/barcode/jasperreports/aspose-barcode-for-jasperreports-18-11-release-notes/
[3]: https://downloads.aspose.com/barcode/jasperreports/new-releases/aspose.barcode-for-jasperreports-18.11/
[4]: https://products.aspose.com/barcode/jasperreports
[5]: https://downloads.aspose.com/barcode/jasperreports
[6]: https://docs.aspose.com/barcode/jasperreports/
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/




