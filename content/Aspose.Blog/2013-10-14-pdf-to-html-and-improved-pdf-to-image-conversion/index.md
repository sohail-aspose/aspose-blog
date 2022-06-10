---
title: 'PDF to HTML and Improved PDF to Image Conversion in Aspose.Pdf for Java 4.3.0'
date: Mon, 14 Oct 2013 19:11:46 +0000
draft: false
url: /2013/10/14/pdf-to-html-and-improved-pdf-to-image-conversion/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert PDF to images in Java', 'convert pdf to html in java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


We are pleased to announce the release of [Aspose.PDF for Java 4.3.0][1]. This new release provides an exciting feature to convert PDF files to HTML format by using just two lines of code. We've previously provided the feature to extract PDF file contents as HTML using the PdfExtractor class' extractTextAsHTML(..) method but the new approach greatly improves the output fidelity.

```
// Load source PDF file
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document("c:/source.pdf");
// Save the file into HTML format
pdfDocument.save("c:/output.html", com.aspose.pdf.SaveFormat.Html);
```

In this new release, we have introduced a separate JAR file, **aspose-pdf-4.3.0-jdk14.jar**, targeted for JDK1.4 and JDK1.5. Furthermore, this release also provides better PDF to image conversion, both in terms of results and performance.

Find out what's new and fixed in [Aspose.PDF for Java 4.3.0][2].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java




