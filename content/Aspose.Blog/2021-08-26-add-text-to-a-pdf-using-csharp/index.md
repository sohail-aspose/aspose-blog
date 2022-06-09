---
title: 'Add Text to a PDF Document using C#'
seoTitle: "Add Text to PDF in C# | Add Transparent Text in PDF using C# VB.NET"
description: "Use .NET PDF API to add text to the PDF files using C# or VB.NET. Add normal or transparent text to the desired page in PDF programmatially."
date: Thu, 26 Aug 2021 23:56:00 +0000
draft: false
url: /2021/08/26/add-text-to-a-pdf-using-csharp/
author: Usman Aziz
summary: '[PDF][1] format is widely used to generate various types of documents such as invoices, financial reports, resumes, etc. In the world of automation, PDF documents are generated and manipulated from within the web or desktop applications. Thereby, in certain cases, you may need to add text to the existing PDF files programmatically. In accordance with that, this article shows **how to add text to PDF documents using C#**.'
tags: ['add text to pdf in csharp', 'add transparent text to pdf in csharp', 'dotnet pdf api']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF.png" alt="Add Text to PDF in C#">}}


[PDF][2] format is widely used to generate various types of documents such as invoices, financial reports, resumes, etc. In the world of automation, PDF documents are generated and manipulated from within the web or desktop applications. Thereby, in certain cases, you may need to add text to the existing PDF files programmatically. In accordance with that, this article shows **how to add text to PDF documents using C#**.

*   [C# API to Add Text to PDF][3]
*   [Add Text to a PDF using C#][4]
*   [Add Text to PDF using TextParagraph][5]
*   [Insert Transparent Text in PDF][6]

## C# API to Add Text to PDF {#API-to-Add-Text-to-PDF}

In order to add text to PDF files dynamically, we will use [Aspose.PDF for .NET][7]. It is a feature-rich API that lets you create and manipulate PDF files from within your .NET applications. You can either [download][8] the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.PDF
```

## Add Text to a PDF using C# {#Add-Text-to-a-PDF}

The following are the steps to add text to a PDF file using C#.

*   Load the PDF file using [Document][10] class.
*   Get the desired page of the PDF into a [Page][11] object.
*   Create a [TextFragment][12] object and set its text, position, font, background color, etc.
*   Create a [TextBuilder][13] object and initialize it with _Page_ object.
*   Use [TextBuilder.AppendText(TextFragment)][14] method to add text to the PDF's page.
*   Save the updated PDF file using [Document.Save(String)][15] method.

The following code sample shows how to add text to a PDF file.

{{< gist aspose-com-gists 9ffb1c9daa703e0eb7e1d03bf7aeb882 "add-text-to-pdf.cs" >}}

## Add Text to PDF using TextParagraph {#Add-Text-to-PDF-using-TextParagraph}

The following are the steps to add text to a PDF file using [TextParagraph][16].

*   Load the PDF file using [Document][17] class.
*   Get the desired page of PDF into a [Page][18] object or add a new one.
*   Create a [TextBuilder][19] object and initialize it with _Page_ object.
*   Create an object of [TextParagraph][20] class.
*   Specify the location of the paragraph using [TextParagraph.Rectangle][21] property.
*   Set formatting options of the _TextParagraph_.
*   Create a [TextFragment][22] object and set its text, position, font, background color, etc.
*   Add the TextFragment to the paragraph using [TextParagraph.AppendLine(TextFragment)][23] method.
*   Add paragraph to the page using [TextBuilder.AppendParagraph(TextParagraph)][24] method.
*   Save the updated PDF file using [Document.Save(String)][25] method.

The following code sample shows how to add text to a PDF using TextParagraph class.

{{< gist aspose-com-gists 9ffb1c9daa703e0eb7e1d03bf7aeb882 "add-text-to-pdf-2.cs" >}}

## Add Transparent Text in PDF in C# {#Insert-Transparent-Text-in-PDF}

Aspose.PDF for .NET also allows adding transparent text to a PDF document, as demonstrated in the following steps.

*   Load the PDF file using [Document][26] class.
*   Get the desired page of PDF into a [Page][27] object or add a new one.
*   Create and initialize a [Graph][28] object.
*   Create a [Rectangle][29] object and initialize it.
*   Set [Rectangle.GraphInfo.FillColor][30] property.
*   Add rectangle to the _Graph_ using [Graph.Shapes.Add(Rectangle)][31] method.
*   Add _Graph_ to the paragraphs collection of the page using [Page.Paragraphs.Add(Graph)][32] method.
*   Create a [TextFragment][33] object and set its [TextState.ForegroundColor][34] property.
*   Add the _TextFragment_ to the page using [Page.Paragraphs.Add(TextFragment)][35] method.
*   Save the updated PDF file using [Document.Save(String)][36] method.

The following code sample shows how to add transparent text to a PDF file.

{{< gist aspose-com-gists 9ffb1c9daa703e0eb7e1d03bf7aeb882 "add-transparent-text-in-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for .NET without evaluation limitations using a [temporary license][37].

## Conclusion

In this article, you have learned how to add text to the existing PDF files using C#. In addition, you have seen how to add transparent text to a PDF dynamically. You can explore more about the C# PDF API using the [documentation][38]. Also, you can post your queries on our [forum][39].

## See Also

*   [Create PDF Files using C# – .NET PDF API][40]
*   [Extract Data from Tables in PDF using C#][41]
*   [Extract Text from PDF using C#][42]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Add-Text-to-PDF
[4]: #Add-Text-to-a-PDF
[5]: #Add-Text-to-PDF-using-TextParagraph
[6]: #Insert-Transparent-Text-in-PDF
[7]: https://products.aspose.com/pdf/net
[8]: https://downloads.aspose.com/pdf/net
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder/methods/appendtext
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph/properties/rectangle
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph/methods/appendline
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder/methods/appendparagraph
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/rectangle
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf/graphinfo/properties/fillcolor
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentstate/properties/foregroundcolor
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[36]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[37]: https://purchase.aspose.com/temporary-license
[38]: https://docs.aspose.com/pdf/net/overview/
[39]: https://forum.aspose.com/
[40]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/
[41]: https://blog.aspose.com/2021/06/10/extract-table-from-pdf-using-csharp/
[42]: https://blog.aspose.com/2020/05/16/extract-text-from-pdf-csharp-vb-net/





