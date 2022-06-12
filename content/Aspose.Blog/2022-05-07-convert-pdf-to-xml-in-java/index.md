---
title: 'Convert PDF Files to XML in Java'
seoTitle: "Convert PDF to XML in Java | PDF to PdfXML or MobiXML in Java"
description: "Use Java PDF API to convert PDF files to XML programmatically in Java. Convert PDF to MobiXML or PdfXML format programmatically as per your requirements."
date: Sat, 07 May 2022 06:42:00 +0000
draft: false
url: /2022/05/07/convert-pdf-to-xml-in-java/
author: Usman Aziz
summary: '[XML][1] is a versatile markup language that is used for multiple purposes, such as data management, web, Office tools, documents, etc. Since XML is convenient to be processed by computer programs, the [PDF][2] documents are often converted into XML formats to get the structured representation of the content. The converted XML uses different tags to represent the PDF document. In this article, you will learn **how to convert a PDF file to XML programmatically in Java**.'
tags: ['Convert PDF to MobiXML Java', 'Convert PDF to PdfXML Java', 'Java API to Convert PDF to XML']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Convert-PDF-to-XML.png" alt="Convert PDF Files to XML in Java">}}


[XML][3] is a versatile markup language that is used for multiple purposes, such as data management, web, Office tools, documents, etc. Since XML is convenient to be processed by computer programs, the [PDF][4] documents are often converted into XML formats to get the structured representation of the content. The converted XML uses different tags to represent the PDF document. In this article, you will learn **how to convert a PDF file to XML programmatically in Java**.

*   [Java API to Convert PDF to XML][5]
*   [Convert PDF to XML][6]
    *   [PDF to MobiXML][7]
    *   [PDF to PdfXML][8]

## Java API to Convert PDF to XML {#API-to-Convert-PDF-to-XML}

[Aspose.PDF for Java][9] is a powerful API for PDF generation and manipulation. Using the API, you can seamlessly create, process, and convert PDF files of simple and complex layouts. We will use this API for PDF to XML conversion in this article. You can [download][10] the API's JAR or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Convert PDF to XML in Java {#Convert-PDF-to-XML}

Aspose.PDF supports the following XML standards for PDF to XML conversion:

*   MobiXML
*   PdfXML

You can choose any of the above-mentioned formats for the converted XML file. So let's proceed to see how to perform PDF to XML conversion within Java applications.

### Convert PDF to MobiXML in Java {#PDF-to-MobiXML}

The following are the steps to convert a PDF to MobiXML format in Java.

*   Load the PDF document using the ********[Document][11]******** class.
*   Convert PDF to XML using **[Document.save(string, SaveFormat)][12]** method and pass **[SaveFormat.MobiXml][13]** as second parameter.

The following code sample shows how to convert a PDF to MobiXML format in Java.

\[gist id="120b54dc4cf2128d84d92a1664b84ad2" file="pdf-to-mobixml.java"\]

### Convert PDF to PdfXML in Java {#PDF-to-PdfXML}

To convert a PDF to PdfXML format, you need to pass **[SaveFormat.PdfXml][14]** as the second parameter of **Document.save(string, SaveFormat)** method. The following code sample shows how to convert a PDF to PdfXML format in Java.

\[gist id="120b54dc4cf2128d84d92a1664b84ad2" file="pdf-to-pdfxml.java"\]

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][15] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert a PDF document to XML in Java. You have seen how to convert a PDF to MobiXML or PdfXML format programmatically. In addition, you can visit the [documentation][16] to read more about Aspose.PDF for Java. In case you would have any questions or queries, you can contact us via our [forum][17].

## See Also

*   [Creating PDF Files from Scratch using Java][18]
*   [Create Graphs and Charts in PDF in Java][19]


[1]: https://docs.fileformat.com/web/xml/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/web/xml/
[4]: https://docs.fileformat.com/pdf/
[5]: #API-to-Convert-PDF-to-XML
[6]: #Convert-PDF-to-XML
[7]: #PDF-to-MobiXML
[8]: #PDF-to-PdfXML
[9]: https://products.aspose.com/pdf/java/
[10]: https://downloads.aspose.com/pdf/java
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[12]: https://reference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-com.aspose.pdf.SaveFormat-
[13]: https://reference.aspose.com/pdf/java/com.aspose.pdf/SaveFormat#MobiXml
[14]: https://reference.aspose.com/pdf/java/com.aspose.pdf/SaveFormat#PdfXml
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/pdf/java/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/
[19]: https://blog.aspose.com/2022/05/24/create-graphs-and-charts-in-pdf-in-java/





