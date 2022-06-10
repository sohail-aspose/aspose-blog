---
title: 'Error Reporting in Text Extraction from PDF in Java'
date: Sun, 07 Jan 2018 21:25:47 +0000
draft: false
url: /2018/01/07/text-extraction-error-reporting-and-pdf-incremental-updates-features/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We are pleased to announce that [Aspose.PDF for Java 17.12][1] is available for download with new features and improvements. In case you are planning to upgrade your existing API to the latest version, we recommend you to please check the release notes of Aspose.PDF for Java 17.12 for an overview of public API changes and improvements. However, the following are some major improvements and fixes in terms of text extraction and document manipulation features.

## Error Reporting in Text Extraction from PDF

While investigating a scenario where a PDF document used PDF Type 3 fonts, it was observed that the TextAbsorber class was not retrieving the text correctly. The reason was that the fonts used in the PDF, contained different encoding and it is not possible to extract text from such documents, by using Adobe Reader itself. We realized the necessity to implement a functionality in the API that such error in the document can be reported. We are pleased to inform you that text extraction error reporting has been implemented for TextAbsorber and TextFragmentAbsorber classes, which is available with [Aspose.PDF for Java 17.12][2]. Following code snippet can be used to detect errors while extracting text from a PDF document:

```
Document pdf = new Document("test.pdf");
TextAbsorber absorber = new TextAbsorber();
absorber.getTextSearchOptions().setLogTextExtractionErrors(true);
pdf.getPages().accept(absorber);
if (absorber.hasErrors()) {
    // Information about found errors and locations is stored in 
    // Errors collection.
    for (TextExtractionError error : absorber.getErrors()) {
      // TextExtractionError object contains information about the
      // text extraction error found during processing concrete 
      // text fragment.
      System.out.println(error);
      System.out.println(String.format("Extracted text: '{0}'",
      error.getExtractedText()));
    }
}
```

## Save PDF document into Stream object using Incremental Updates

It was observed that when you load a PDF document from binary, manipulate it (i.e add some annotations) and save it to a different binary – the content of the PDF document was used to be totally changed. In order to avoid such issues, we have implemented an additional method i.e **saveIncrementally()** into the Document class. Now you will be able to save the document into a Stream object, using Incremental Updates.

## Miscellaneous Fixes

As it always recommended to use the latest release of our APIs as they include the latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 17.12.][3]

*   [Home page for Aspose.PDF for Java][4]
*   [Download Aspose.PDF for Java][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][7]– help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/17.12/
[2]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/17.12/
[3]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf/17.12/
[4]: https://products.aspose.com/pdf/java
[5]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf/17.12/
[6]: https://forum.aspose.com/c/pdf
[7]: https://docs.aspose.com/display/pdfjava/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




