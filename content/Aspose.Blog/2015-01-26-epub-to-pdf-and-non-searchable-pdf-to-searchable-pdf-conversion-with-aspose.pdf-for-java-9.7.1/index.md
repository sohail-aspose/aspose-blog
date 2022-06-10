---
title: 'Convert EPUB to PDF, Convert Non-searchable PDF to Searchable PDF in Java using Aspose.PDF for Java'
date: Mon, 26 Jan 2015 15:48:51 +0000
draft: false
url: /2015/01/26/epub-to-pdf-and-non-searchable-pdf-to-searchable-pdf-conversion-with-aspose.pdf-for-java-9.7.1/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert EPUB to PDF in Java', 'Convert non-searchable PDF to searchable PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


It gives us an immense pleasure to announce the release of of [Aspose.PDF for Java 9.7.1][1] which provides new features and enhancements previously requested by other customers. Along these new features and enhancements, many of the issues reported in previous release versions are also resolved, which make this new release more powerful and robust as compared to earlier releases.

## Convert EPUB to PDF in Java

EPUB (short for electronic publication) is a free and open e-book standard from the International Digital Publishing Forum (IDPF). Files have the extension .epub. The conversion of EPUB to PDF has been supported in Aspose.Pdf for .NET for quite some time. So under the same vision of making both siblings identical in features, the conversion of EPUB to PDF is now supported in Aspose.Pdf for Java. For further details, please visit Convert EPUB File to PDF Format

```
//Instantiate LoadOption object using EPUB load option
com.aspose.pdf.EpubLoadOptions optionsepub = new com.aspose.pdf.EpubLoadOptions();
//Create Document object
com.aspose.pdf.Document docepub = new com.aspose.pdf.Document("C:\\source.epub", optionsepub);
//Save the resultant PDF document
docepub.save("C:\\resultant.pdf");
```

## Convert Non-searchable PDF to Searchable PDF in Java

A PDF file may consist of Text, Image, Attachments, Annotations, Graphs etc elements. In case we have an image file converted to PDF format and we have a requirement to manipulate/extract the text contents from Image PDF, it is not possible in a simple manner. Even Adobe reader cannot provide the feature to extract text contents from Image PDF. In order to accomplish this requirement, we need to perform OCR over image inside PDF file and then extract those contents for further manipulation. In this new release, we have supported the feature to convert non-searchable (Image PDF) to searchable PDF document and it can be accomplish with the help of [Google tesseract OCR][2]. For further details, please visit [Converting non searchable PDF to searchable PDF document][3].

As well as the enhancements and features discussed above, there have been numerous fixes related to recently introduced PDF to DOC conversion, PDF to Excel conversion, PDF to HTML conversion, PDF to PDF/A conversion, XPS to PDF conversion, PDF to TIFF conversion, text replacement, text extraction, rendering PDF files to XPS, creating TOCs in PDF files, and printing PDFs with embedded fonts. Please download and try the latest [Aspose.PDF for .NET 9.7.1][4] release.




[1]: https://downloads.aspose.com/pdf/java
[2]: http://en.wikipedia.org/wiki/Tesseract_%28software%29
[3]: http://docs.aspose.com/display/pdfjava/Converting+non+searchable+PDF+to+searchable+PDF+document
[4]: https://downloads.aspose.com/pdf/java




