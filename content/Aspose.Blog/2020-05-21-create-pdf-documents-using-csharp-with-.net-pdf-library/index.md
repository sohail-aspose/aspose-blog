---
title: 'Create PDF Files using C# with .NET PDF Library'
seoTitle: ""
description: ""
date: Thu, 21 May 2020 17:20:45 +0000
draft: false
url: /2020/05/21/create-pdf-documents-using-csharp-with-.net-pdf-library/
author: Usman Aziz
summary: ''
tags: ['.NET PDF Library', 'Create PDF Documents using Csharp', 'Csharp PDF Library', 'Generate PDF Documents using Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-PDF-Documents-using-C.jpg" alt="Create PDF Documents using C#">}}


[PDF][1] is a platform-independent document format that keeps the formatting and layout of its content consistent across different operating systems or machines. This is the reason various organizations use PDF format for generating invoices, receipts, reports, and other business documents dynamically. Aspsoe.PDF for .NET is a PDF library that helps you implement PDF automation in .NET applications. It allows you to create, edit, parse and convert PDF files programmatically using C# or VB.NET. In this article, I'll cover PDF generation features and show you **how to create PDF files from scratch using C#**.

I'll start by creating a simple PDF document and then proceed to add other elements to the document. The following is the list of features I am going to demonstrate in this article.

*   [Create a PDF document using C#][2]
*   [Apply text formatting in PDF using C#][3]
*   [Create a multi-column PDF using C#][4]
*   [Insert an image in a PDF using C#][5]
*   [Create a table in a PDF using C#][6]
*   [Add Hyperlinks to a PDF using C#][7]
*   [Add bookmarks to a PDF using C#][8]

## C# PDF Library - Installation

You can install Aspose.PDF for .NET using [NuGet Package Manager][9] or Package Manager Console using the following command. Alternatively, it can be downloaded from the [Downloads][10] section.

```
Install-Package Aspose.Pdf
```

## Create a PDF File using C# {#Create-a-PDF-document-using-CSharp}

Lets first create a PDF document containing a text fragment. The following are the steps to create a simple PDF document from scratch.

*   Create an instance of [Document][11] class.
*   Add a new [Page][12] to the [Pages][13] collection of the document.
*   Add a new [TextFragment][14] to the paragraphs of the PDF.
*   Create the PDF file using [Document.Save()][15] method.

The following code sample shows how to create a PDF file using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "create-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-using-C.jpg" alt="create pdf using C#">}}


## Apply Text Formatting in PDF using C# {#Apply-text-formatting-in-PDF-using-CSharp}

Let's now check out how to add text to a PDF document and use different formatting options. The following are the steps to perform this operation.

*   Use [Document][16] class to create a new PDF document or load an existing one.
*   Access the [Page][17] you want to place the text on.
*   Create an object of [TextFragment][18] and set the text and other formatting options such as position, font, color, size, etc.
*   Use the [TextBuilder][19] class to add the _TextFragment_ object to the page.
*   Use the [Document.Save()][20] method to create the PDF document.

The following code sample shows how to add formatted text in a PDF file using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "add-formatted-text-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-Text-Formatting-C.jpg" alt="create pdf with formatted text using C#">}}


## Create a Multi-Column PDF using C# {#Create-a-multi-column-PDF-using-CSharp}

We often see that the text in newspapers, research articles, and other types of document is divided into two or more columns. In order to achieve this text division, Aspose.PDF for .NET allows creating a multi-column PDF. The following are the steps to create a multi-column PDF.

*   Create a new PDF document using [Document][21] class.
*   Add a new [Page][22] to the document using [Document.Pages.Add()][23] method.
*   Set page margins using the [Document.PageInfo.Margin][24] properties.
*   Create a new [FloatingBox][25] object and set [ColumnCount][26], [ColumnSpacing][27], and [ColumnWidths][28] properties.
*   Create a new [TextFragment][29] and set its text.
*   Add _TextFragment_ to the _FloatingBox_ using [FloatingBox.Paragraphs.Add()][30].
*   Add _FloatingBox_ to the page using [Page.Paragraphs.Add()][31].
*   Save the PDF using the [Document.Save()][32] method.

The following code sample shows how to create a multi-column PDF using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "create-multicolumn-pdf.cs" >}}



{{< figure align=center src="images/Create-multicolumn-PDF-using-C.jpg" alt="create multi-column pdf using C#">}}


## Insert Image in a PDF using C# {#Insert-an-image-in-a-PDF-using-CSharp}

The following steps demonstrate how to insert images in PDF documents.

*   Create a new PDF document or open an existing one using [Document][33] class.
*   Get the page you want to insert an image in.
*   Add the image to the page's images.
*   Use [GSave][34], [ConcatenateMatrix][35], and [Do][36] operators to place the image on the page.
*   Save the PDF document using [Document.Save()][37] method.

The following code sample shows how to insert an image in PDF using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "insert-image-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-Image-C.jpg" alt="insert image in PDF using C#">}}


## Create Table in a PDF File using C# {#Create-a-table-in-a-PDF-document-using-CSharp}

The table is used to organize the data in the form of rows and columns and to provide a quick overview of the information. In order to create a table in the PDF document, follow the below steps.

*   Create an object of [Document][38] class to create a new PDF or load an existing one.
*   Access the page you want to create a table in.
*   Create an instance of [Table][39] class.
*   Set the table's border and cells' border using the [BorderInfo][40] class.
*   Create and add a new [Row][41] to the [Table.Rows][42] collection.
*   Add cells to the [Row.Cells][43] collection.
*   Add the table to the page using [Page.Paragraphs.Add()][44] method.
*   Save the PDF document using [Document.Save()][45] method.

The following code sample shows how to create a table in PDF using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "create-table-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-Table-C.jpg" alt="create table in pdf using C#">}}


## Add Annotation in a PDF using C# {#Create-annotation-in-a-PDF-file-using-CSharp}

Annotations are graphical objects that are used to provide additional information about the content in the PDF documents. PDF format supports various annotations including text, highlight, line, notes, and etc. The following are the steps to add an annotation in a PDF document.

*   Create a new PDF document or load an existing one.
*   Choose the page to which you want to add an annotation.
*   Create a new annotation such as [TextAnnotation][46], [LineAnnotation][47], [HighlightAnnotation][48], etc.
*   Set the properties of the annotation.
*   Add annotation to the [Page.Annotations][49] collection.
*   Generate the PDF using the [Document.Save()][50] method.

The following code sample shows how to add an annotation to PDF using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "add-annotation-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-annotation-C.jpg" alt="add annotation in PDF using C#">}}


## Add Hyperlinks to a PDF File using C# {#Add-Hyperlinks-to-a-PDF-using-CSharp}

You can also add hyperlinks to a PDF document using the Link Annotation. The following are the steps to perform this operation.

*   Create a new [Document][51] object.
*   Access the page where you want to add the hyperlink.
*   Create an instance of the [LinkAnnotation][52] class.
*   Set _LinkAnnotation_ object's properties including the action URI.
*   Add the link to the [Page.Annotations][53] collection.
*   Use the [FreeTextAnnotation][54] class to set the text of the hyperlink.
*   Add _FreeTextAnnotation_ object to the [Page.Annotations][55] collection.
*   Create PDF document using [Document.Save()][56] method.

The following code sample shows how to add a hyperlink to a PDF document using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "add-hyperlink-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-HyperlinkC.jpg" alt="add hyperlink in PDF using C#">}}


## Create Bookmarks in a PDF using C# {#Add-bookmarks-to-a-PDF-using-CSharp}

Bookmarks are used to navigate to a particular section or page in PDF documents. Aspose.PDF for .NET allows you to add or manipulate bookmarks. The following are the steps to create and add a bookmark in a PDF document.

*   Create a PDF document or open an existing one.
*   Create a new bookmark object using the [OutlineItemCollection][57] class.
*   Add bookmarks to [Document.Outlines][58] collection.
*   Create the PDF document using [Document.Save()][59] method.

The following code sample shows how to create a PDF document with bookmarks using C#.

{{< gist aspose-com-gists c34d6130720473e294257b67aee03a1f "create-bookmark-in-pdf.cs" >}}



{{< figure align=center src="images/Create-PDF-with-Bookmarks-C.jpg" alt="create bookmark in PDF using C#">}}


## Conclusion

In this article, I have shown you how to create PDF files from scratch using C#. The step by step guide and code samples demonstrate how to add text, image, table, annotation, hyperlink, and bookmarks in the PDF files programmatically. You can explore other features of Aspose's .NET PDF Library using the [documentation][60].

## See Also

*   [Create PDF Documents using C++][61]




[1]: https://wiki.fileformat.com/view/pdf/
[2]: #Create-a-PDF-document-using-CSharp
[3]: #Apply-text-formatting-in-PDF-using-CSharp
[4]: #Create-a-multi-column-PDF-using-CSharp
[5]: #Insert-an-image-in-a-PDF-using-CSharp
[6]: #Create-a-table-in-a-PDF-document-using-CSharp
[7]: #Add-Hyperlinks-to-a-PDF-using-CSharp
[8]: #Add-bookmarks-to-a-PDF-using-CSharp
[9]: https://nuget.org/packages/Aspose.pdf
[10]: https://downloads.aspose.com/pdf/net
[11]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[16]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[21]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pageinfo
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/floatingbox
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/columninfo/properties/columncount
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/columninfo/properties/columnspacing
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf/columninfo/properties/columnwidths
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf/floatingbox/properties/paragraphs
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[33]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/gsave
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/concatenatematrix
[36]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/do
[37]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[38]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[39]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[40]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[41]: https://apireference.aspose.com/pdf/net/aspose.pdf/row
[42]: https://apireference.aspose.com/pdf/net/aspose.pdf/table/properties/rows
[43]: https://apireference.aspose.com/pdf/net/aspose.pdf/row/properties/cells
[44]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[45]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[46]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/textannotation
[47]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/lineannotation
[48]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/highlightannotation
[49]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[50]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[51]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[52]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation
[53]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[54]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/freetextannotation
[55]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[56]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[57]: https://apireference.aspose.com/pdf/net/aspose.pdf/outlineitemcollection
[58]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/outlines
[59]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[60]: https://docs.aspose.com/display/pdfnet/Product+Overview
[61]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





