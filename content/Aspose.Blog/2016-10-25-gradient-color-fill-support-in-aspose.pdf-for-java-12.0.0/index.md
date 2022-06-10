---
title: 'Gradient Color Fill Support in Aspose.Pdf for Java 12.0.0'
date: Tue, 25 Oct 2016 19:38:31 +0000
draft: false
url: /2016/10/25/gradient-color-fill-support-in-aspose.pdf-for-java-12.0.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[![][1]](http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png)We are pleased to announce [Aspose.Pdf for Java 12.0.0][2] release. As we know it is ported version of Aspose.Pdf for .NET, so it includes all the enhancements and improvements from the corresponding .NET version along with the fixes of the bugs reported in previous versions of Aspose.Pdf for Java by our customers. It contains support of Gradient Color fill besides enhancement of PDF to DOC conversion feature. In addition to above enhancement, we have some important improvements regarding Printing on Linux, PDF to PDFA, XML to PDF and Redaction Annotation. Please check release notes of Aspose.Pdf for Java 12.0.0 for complete list of bug fixed.

Please note if you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section of current release and other intermediate releases, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these enhancements/Improvements:

## Gradient Color Fill Support

We have added Gradient Color fill support in this release. For this requirement, we have introduced PatternColorSpace property in com.aspose.pdf.Color class and GradientAxialShading class added in com.aspose.pdf.drawing package. Now we can fill Graph object with Gradient Color as following:

```
 Document doc = **new** Document();

Page page = doc.getPages().add();

com.aspose.pdf.drawing.Graph graph = **new** com.aspose.pdf.drawing.Graph(300, 300);

page.getParagraphs().add(graph);

com.aspose.pdf.drawing.Rectangle rect = **new** com.aspose.pdf.drawing.Rectangle(0, 0, 300, 300);

graph.getShapes().add(rect);

rect.getGraphInfo().setFillColor(**new** com.aspose.pdf.Color());

com.aspose.pdf.drawing.GradientAxialShading gradientAxialShading = **new** com.aspose.pdf.drawing.GradientAxialShading(com.aspose.pdf.Color._getRed_(), com.aspose.pdf.Color._getBlue_());

gradientAxialShading.setStart(**new** Point(0, 0));

gradientAxialShading.setEnd(**new** Point(300, 300));

rect.getGraphInfo().getFillColor().setPatternColorSpace(gradientAxialShading);

doc.save("GradientFill.pdf"); 
```

## Default Image Resolution of DOC(X) Document

We have received some queries regarding rendering quality of PDF to DOC(X) conversion. So we have set default ImageResolution to 300 dpi in this release. It will increase the output file size but for customers rendering quality of resultant DOC(X) is more important than file size. However, if required we can change the resolution of resultant DOC(X) as following:

```
 com.aspose.pdf.DocSaveOptions saveOptions = **new** com.aspose.pdf.DocSaveOptions();

saveOptions.setFormat(com.aspose.pdf.DocSaveOptions.DocFormat._Doc_);

saveOptions.setMode(com.aspose.pdf.DocSaveOptions.RecognitionMode._Flow_);

saveOptions.setRecognizeBullets(**true**);

saveOptions.setImageResolutionX(150);

saveOptions.setImageResolutionY(150); 
```

## Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.Pdf for Java][3]
*   [Download Aspose.Pdf for Java][4]
*   [Aspose.Pdf product family forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.Pdf for Java online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png "aspose_pdf-for-java"
[2]: http://www.aspose.com/downloads/pdf/java/new-releases/aspose.pdf-for-java-12.0.0/
[3]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[4]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[5]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[6]: https://blog.aspose.com/ "Aspose.Pdf for Java Blog Subscription"
[7]: https://github.com/asposepdf/Aspose_Pdf_JAVA




