---
title: 'Convert PDF to PDFA efficiently with  Aspose.PDF for Java'
date: Sat, 27 Aug 2016 04:34:29 +0000
draft: false
url: /2016/08/27/improved-conversion-of-pdf-to-pdfa-in-aspose.pdf-for-java-11.8.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java.jpg" alt="">}}


We are pleased to announce [Aspose.Pdf for Java 11.8.0][1] maintenance release. This version includes PDF to PDFA conversion improvement in addition to the improvements/enhancements made in its equivalent .NET version. We have fixed number of issues in this release, reported by our customers in previous releases. Some of these are PDF to PDF/A, PDF to HTML, PDF to DOC, Printing issue on iSeries and some others. Please check release notes of Aspose.Pdf for Java 11.8.0 for complete list of bug fixed.

The following section describes some important improvements:

## **PDF to PDFA conversion**

We have improved image rendering logic in PDF to PDFA conversion in this release, that fixed a lot of image related issues in PDFA.

## **Printing issues on non Windows OS**

We have been reported some printing issues on non Windows OS, in previous versions. We have fixed these issues PdfViewer class in current release and it will improve the API reliability.

## Public API Changes

The basic API change in this release is removal of Interfaces namespace.

Changes in class **com.aspose.XFA**:

**added method**

*   public HashMap<String, String> getFieldsWithTextValuesMap()

Changes in class **com.aspose.pdf.PdfFormatConversionOptions**:

**added method**

*   public boolean isLowMemoryMode()
*   public void setLowMemoryMode(boolean value)

Changes in class **com.aspose.pdf.FontSubstitution**:

**added method**

*   public FontDefinition getSubstitutionFontDefinition()

Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.Pdf for Java][2]
*   [Download Aspose.Pdf for Java][3]
*   [Aspose.Pdf product family forum][4] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.Pdf for Java online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][5] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/pdf/java/new-releases/aspose.pdf-for-java-11.8.0/
[2]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[3]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[5]: https://blog.aspose.com/ "Aspose.Pdf for Java Blog Subscription"
[6]: https://github.com/asposepdf/Aspose_Pdf_JAVA




