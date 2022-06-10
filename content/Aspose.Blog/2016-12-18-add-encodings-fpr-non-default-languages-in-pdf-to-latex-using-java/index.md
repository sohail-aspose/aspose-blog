---
title: 'Add Encodings for Non-Default Languages in PDF to Latex using Java'
date: Sun, 18 Dec 2016 16:28:00 +0000
draft: false
url: /2016/12/18/add-encodings-fpr-non-default-languages-in-pdf-to-latex-using-java/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We are pleased to announce [Aspose.PDF for Java 16.11.0][1] release. This version of Aspose.Pdf for Java includes all the features and enhancements introduced it its corresponding .NET version i.e. Aspose.Pdf for .NET 16.11.0 along with additional features. Some of the new features of this release are support of Concatenation progress status, get text width dynamically and support to add encoding of non-default languages in PDF to Latex conversion.. In addition to above enhancement, we have some important improvements regarding PDF to DOCX/DOC, Printing issue on Linux, PDF to PPTX along with many other fixes that makes it more stable and reliable version. Please check [release notes of Aspose.PDF for Java 16.11.0][2] for complete list of bug fixed.

Please note if you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes section of current release][3] and other intermediate releases, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added enhancements.

## Support of Concatenation Progress Status

We have received a requirement to know the progress status of PDF files Concatenation process, that how much process is completed and is the file generation/concatenation completed or not?. We have implemented ConcatenationProgressHandler to check the status of concatenation. Please check the [documentation link][4] for details and sample code snippet.

## Add Encoding for Non-Default Languages in PDF to Latex

While converting PDF to Latex, we need to use non-default languages specific font encoding for the conversion. We have introduced a property addFontEncs in LateXSaveOptions class for the purpose. Here is an example of adding Cyrillic encoding in PDF to Latex conversion.

```
Document doc2 = new com.aspose.pdf.Document("Test.pdf");

com.aspose.pdf.LaTeXSaveOptions opt = new com.aspose.pdf.LaTeXSaveOptions();

opt.addFontEncs("T2A", "T2B");

doc2.save("Test.tex", opt);
```

## Get text width dynamically

Some of the customers need features to calculate text width dynamically. Now with this release, we can [get text width dynamically][5] with use of measureString() method. We can invoke measureString() method of com.aspose.pdf.Font or com.aspose.pdf.TextState classes (or both)

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][6]
*   [Download Aspose.PDF for Java][7]
*   [Aspose.PDF product family forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][9] – Help documentation and API reference documents.
*   [Enable Blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/pdf/java/new-releases/aspose.pdf-for-java-16.10.0/
[2]: http://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+16.11.0+Release+Notes
[3]: http://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+16.11.0+Release+Notes
[4]: http://docs.aspose.com/display/pdfjava/To+Check+Concatenation+Status
[5]: http://docs.aspose.com/display/pdfjava/To+get+text+width+dynamically
[6]: https://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[9]: http://docs.aspose.com/display/pdfjava/Home
[10]: https://blog.aspose.com/
[11]: https://github.com/asposepdf/Aspose_Pdf_JAVA




