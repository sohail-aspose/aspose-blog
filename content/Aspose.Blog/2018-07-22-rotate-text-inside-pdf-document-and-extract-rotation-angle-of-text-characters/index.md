---
title: 'Rotate Text in PDF Document and Convert PDF to XLSX in Java'
date: Sun, 22 Jul 2018 22:46:02 +0000
draft: false
url: /2018/07/22/rotate-text-inside-pdf-document-and-extract-rotation-angle-of-text-characters/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Convert PDF to Excel XLSX in Java', 'Extract rotation angle of text in PDF', 'Rotate text in PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We are pleased to announce the monthly release of [Aspose.PDF for Java 18.6][1]. This release includes some useful features including rotating text in PDF and converting PDF to XLSX. In order to get an idea about all new features and bug fixes incorporated in this release, please check the [release notes page of Aspose.PDF for Java 18.6][2]. In case you are planning to upgrade your existing version to the latest one, we recommend you please check the Public API Changes section in release notes of the API. This way you will have an idea about what has been changed and added new in the latest release.

The following section provides insights into major new features available in Aspose.PDF for Java 18.6.

## Rotate Text in PDF using Java

Adding text with a rotation angle can be an important requirement in particular scenarios of text generation in PDF. In order to add text with rotation in PDF document, you can use the _setRotation()_ method of _TextState_ Class to specify the rotation angle of the text.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-pdf-Text-AddRotatedTextInPDF-1.java" >}}

For more information about this new feature, please check the following article in API documentation:

*   [Add Rotated Text inside PDF document][3]

## Determine Rotation Angle of Text Characters

Along with the functionality of adding rotated text inside PDF, extraction of that text and determining rotation angle of text characters has also been implemented in this release of the API. TextFragmentAbsorber class has further been enhanced to support the extraction of the rotation angle of text characters.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-pdf-Text-ExtractRotatedText.java" >}}

You can check the following article in the API documentation for further details regarding this feature.

*   [Extract Rotated Text and Rotation Angle of Text Characters][4]

## Convert PDF to XLSX in Java

PDF to XLS as well as other file format conversion was already supported in Aspose.PDF for Java. However, a new conversion feature i.e. PDF to XLSX has been introduced in this release of the API.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-CovertPDFtoXLSX.java" >}}

In order to use this feature of the API, please read the following article:

*   [Convert PDF to XLSX format][5]

## Important API Changes

All descendants of com.aspose.pdf.Operator has been moved under the namespace com.aspose.pdf.operators. Thus 'new com.aspose.pdf.operators.GSave()' should be used instead of 'new com.aspose.pdf.Operator.GSave()'. While upgrading to the latest version of the API, you will need to upgrade your existing code where you were using the previous com.aspose.pdf.Operator namespace.

## Miscellaneous Fixes

Along with the features and enhancements mentioned above, followings are useful improvements and bug fixes included in the latest release of API:

*   PDF to HTML Conversion has been improved in terms of visibility and formatting of symbols
*   Fonts handling and watermark rendering have been improved further
*   Improved memory consumption by API methods and calls
*   Worked over formula based fields while converting from XFA to Standard AcroForms
*   Consistency of text format has been maintained while converting PDF to PDF/A
*   Redaction Annotation feature has been further improved
*   Worked over producing better results while extracting bookmarks from PDF

As it is always recommended to use the latest release of our API’s because they include the latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 18.6.][6]

*   [Home page for Aspose.PDF for Java][7]
*   [Download Aspose.PDF for Java 18.6][8]
*   [Aspose.PDF product family forum][9] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][10]– Help documentation and API reference documents.
*   [Enable Blog Subscription][11] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[2]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.6+Release+Notes
[3]: https://docs.aspose.com/
[4]: https://docs.aspose.com/display/pdfjava/Extract+Text+from+PDF#ExtractTextfromPDF-ExtractRotatedTextandRotationAngleofTextCharacters
[5]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+Excel+XLS+and+XLSX
[6]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[7]: https://products.aspose.com/pdf/java
[8]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[9]: https://forum.aspose.com/c/pdf
[10]: https://docs.aspose.com/display/pdfjava/Home
[11]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




