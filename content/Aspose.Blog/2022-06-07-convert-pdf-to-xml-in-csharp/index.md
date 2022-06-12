---
title: 'Convert PDF Files to XML in C# .NET'
seoTitle: "Convert PDF to XML in C# .NET | PDF to PdfXML or MobiXML in C#"
description: "Use .NET PDF API to convert PDF files to XML programmatically in C#. Convert PDF to MobiXML or PdfXML format as per your requirements."
date: Tue, 07 Jun 2022 04:52:00 +0000
draft: false
url: /2022/06/07/convert-pdf-to-xml-in-csharp/
author: Usman Aziz
summary: "XML is a well-known markup language similar to HTML. However, its uses spread across multiple scenarios such as data management, web, office tools, documents, etc. In particular cases, the PDF documents are converted into XML files to get the structured representation of the content. Thus, the tag-based representation of the PDF documents can be processed more conveniently for different purposes. Accordingly, in this article, you will learn **how to convert a PDF file to XML programmatically in C#**."
tags: ['convert pdf to mobixml in csharp', 'convert pdf to pdfxml in csharp', 'convert pdf to xml in csharp', 'generate xml from pdf in csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Convert-PDF-to-XML.png" alt="Convert PDF Files to XML in C#">}}


[XML][3] is a well-known markup language similar to HTML. However, its uses spread across multiple domains such as data management, web, Office tools, documents, etc. In particular cases, the [PDF][4] documents are converted into XML files to get the structured representation of the content. Thus, the tag-based representation of the PDF documents can be processed more conveniently for different purposes. Accordingly, in this article, you will learn **how to convert a PDF file to XML programmatically in C#**.

*   [.NET API to Convert PDF to XML][5]
*   [Convert PDF to XML][6]
    *   [PDF to MobiXML][7]
    *   [PDF to PdfXML][8]

## C# .NET API to Convert PDF to XML {#API-to-Convert-PDF-to-XML}

For PDF to XML conversion, we will use [Aspose.PDF for .NET][9]. It is a popular API that allows you to create and process PDF files from within .NET applications. Furthermore, it provides a high fidelity converter to convert PDF files to other formats. You can [download][10] the API's binaries or install it using [NuGet][11].

```
PM> Install-Package Aspose.PDF
```

## Convert PDF to XML in C# {#Convert-PDF-to-XML}

Aspose.PDF for .NET allows the conversion of PDF documents to the following XML standards:

*   MobiXML
*   PdfXML

Let's see how to convert a PDF to each of the above-mentioned XML formats using Aspose.PDF for .NET.

### PDF to MobiXML in C# {#PDF-to-MobiXML}

The following are the steps to convert a PDF to MobiXML format in C#.

*   Load the PDF document using the ****[Document][12]**** class.
*   Convert PDF to XML using **[Document.Save(string, SaveFormat)][13]** method and pass **[SaveFormat.MobiXml][14]** as second parameter.

The following code sample shows how to convert a PDF to XML with MobiXML format in C#.

\[gist id="19c1f480f90973eb5f097b3963ca169d" file="pdf-to-mobixml.cs"\]

### PDF to PdfXML in C# {#PDF-to-PdfXML}

To convert a PDF to PdfXML format, you need to pass **SaveFormat.PdfXml** as the second parameter of **Document.Save(string, SaveFormat)** method. The following code sample shows how to convert a PDF to PdfXML format in C#.

\[gist id="19c1f480f90973eb5f097b3963ca169d" file="pdf-to-pdfxml.cs"\]

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][15] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert a PDF document to XML in C#. Furthermore, we have explicitly covered how to convert a PDF to MobiXML or PdfXML format programmatically. In addition, you can explore more about .NET PDF API using the [documentation][16]. In case you would have any questions or queries, you can contact us via our [forum][17].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][18]
*   [Extract Images from PDF using C#][19]
*   [Create PDF File from Images using C#][20]


[1]: https://docs.fileformat.com/web/xml/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/web/xml/
[4]: https://docs.fileformat.com/pdf/
[5]: #API-to-Convert-PDF-to-XML
[6]: #Convert-PDF-to-XML
[7]: #PDF-to-MobiXML
[8]: #PDF-to-PdfXML
[9]: https://products.aspose.com/pdf/net/
[10]: https://downloads.aspose.com/pdf/net/
[11]: http://nuget.org/packages/Aspose.PDF
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://reference.aspose.com/pdf/net/aspose.pdf.document/save/methods/6
[14]: https://reference.aspose.com/pdf/net/aspose.pdf/saveformat
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/pdf/net/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[19]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[20]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/





