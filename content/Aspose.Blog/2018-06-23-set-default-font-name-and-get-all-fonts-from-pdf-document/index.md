---
title: 'Set Default Font Name and Get All Fonts from PDF Document in Java'
date: Sat, 23 Jun 2018 20:36:42 +0000
draft: false
url: /2018/06/23/set-default-font-name-and-get-all-fonts-from-pdf-document/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'change default font in pdf', 'find fonts in PDF', 'get fonts from pdf', 'set default font in PDF java', 'set default font in pdf']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="Set default font in PDF in Java">}}


We at Aspose are glad to announce a new release of Aspose.PDF for Java. [Aspose.PDF for Java 18.5][1] is available on [Aspose Artifactory][2] for download. In the latest release our Java API, we have introduced the feature of setting default font in PDF documents. Furthermore, you'll now be able to get all the fonts from the PDF in Java. Several bug fixes and performance improvements have also been made in this release of the API. A detailed overview of API improvements and changes has been given over the [release notes page][3] of [Aspose.PDF for Java 18.5][4].

## Set Default Font Name in PDF

Usually, Aspose.PDF for Java API used to replace fonts with the default font in PDF documents when specific fonts were not present or installed in the device where document was being generated. Therefore, we have investigated for feasibility; if a font is used and embedded into the document, the output document should have same font – instead of being replaced by some default font. We have implemented this feature by introducing **setDefaultFontName()** method in [**PdfSaveOptions**][5] class. An example with complete code snippet is also showcased in API documentation for how to set the default font in a PDF document:

*   [Set Default Font Name while Saving PDF][6]

## Get all Fonts from PDF File

One of the excited features in Aspose.PDF for Java 18.5 is to get all fonts from PDF document programmatically. With this release of the API, you can get all fonts by using **getAllFonts()** method. An example with complete Java code snippet is given at following link of the API documentation:

*   [Get All Fonts from PDF Document][7]

## Miscellaneous Fixes

Along with the features, which have been announced above, we have also fixed the following reported bugs in this release of the API:

*   NullPointerException when saving PDF as HTML
*   Aspose.Pdf 18.4 throws exception "Incomplete private key - missing CRT." when signing document with .pfx file
*   PDF to HTML: Extra space is being rendered with commos
*   Text goes beyond the page after replacing
*   PDF to HTML - Hyperlinks are removed in resultant file

As it is always recommended to use latest release of our API’s because they include latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 18.5.][8]

*   [Home page for Aspose.PDF for Java][9]
*   [Download Aspose.PDF for Java 18.5][10]
*   [Aspose.PDF product family forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][12]– Help documentation and API reference documents.
*   [Enable Blog Subscription][13]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.5
[2]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/
[3]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.5+Release+Notes
[4]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.5
[5]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/PdfSaveOptions
[6]: https://docs.aspose.com/display/pdfjava/Formatting+PDF+Document#FormattingPDFDocument-SetDefaultFontNamewhileSavingPDF
[7]: https://docs.aspose.com/display/pdfjava/Formatting+PDF+Document#FormattingPDFDocument-GetAllFontsfromPDFDocument
[8]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.5
[9]: https://products.aspose.com/pdf/java
[10]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.5
[11]: https://forum.aspose.com/c/pdf
[12]: https://docs.aspose.com/display/pdfjava/Home
[13]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




