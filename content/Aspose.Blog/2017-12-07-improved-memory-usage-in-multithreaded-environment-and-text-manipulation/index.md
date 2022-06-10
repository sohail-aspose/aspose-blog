---
title: 'Improved Memory usage in Multithreaded Environment and Text Manipulation'
date: Thu, 07 Dec 2017 19:27:32 +0000
draft: false
url: /2017/12/07/improved-memory-usage-in-multithreaded-environment-and-text-manipulation/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Improved Memory Usage for PDF', 'Multithreaded Text Manipulation in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We always aspire to deliver an API with enhancements and improvements and our product team has been working hard to implement new features as well as improving performance of the API. We are pleased to announce that [Aspose.PDF for Java 17.11][1] is available for download with exciting features and improvements. Please visit [release notes][2] of Aspose.Pdf for Java 17.11 for an overview of public API changes and improvements. However, please check following major improvements regarding memory usage and text manipulations in the new release of the API.

## Memory Usage in Multithreaded Environment

In the previous version(s) of the API, the API used to raise an exception when the heap memory occupation was close to the limit. It has specifically been observed while converting PDF documents with a HOCR callback in multithreaded environments. The product team has been working on implementing functionality to extract images from PDF in the raw format, so the **memory consumption was decreased to significant level**. The existing method to convert PDF with HOCR callback has been improved as follows:

```
pdf.convert(callback, false, true);
```

In the above line of code, the first boolean parameter notifies that searchable text should be invisible with the false value – whereas the second boolean parameter is used to notify that the internal images should be returned as they are, with the true value. This enhancement in the convert() method has brought a significant improvement in the memory consumption and it also has been tested that using this approach, program has become faster twice than with the previous method.

## Identify Underline Text and improved Replacement options

It was observed during replacing/removing underline text from PDF documents, that text was used to be replaced/removed but the underline stayed drawn. We have implemented mechanism that starts a searching for text underlining in the source document on any text edit operation. TextFragmentAbsorber removes the underline from text, where underline is not the part of actual text but a graphical element and replace it with original underline like it is added through TextState of the original TextFragment.

After that, any text edit operation will be performed with an affected fragment (or segment) in the same way if it was underlined by using TextState.Underline property of TextFragment (or TextSragment). In order to enable the described mechanism you can set **ToAttemptGetUnderlineFromSource** to 'true' in TextEditOptions option of TextFragmentAbsorber (or PdfContentEditor) object.

## Miscellaneous fixes

As it always recommended to use latest release of our API’s as they include latest features / improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.Pdf for Java 17.11.][3]

*   [Home page for Aspose.PDF for Java][4]
*   [Download Aspose.PDF for Java][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for Java online documentation][7]– help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.



[1]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf/17.11/
[2]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.11+Release+Notes
[3]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf/17.11/
[4]: https://products.aspose.com/pdf/java
[5]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf/17.11/
[6]: https://forum.aspose.com/c/pdf
[7]: https://docs.aspose.com/display/pdfjava/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




