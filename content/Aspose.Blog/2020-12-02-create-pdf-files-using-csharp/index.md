---
title: 'Create PDF Files using C# - .NET PDF API'
seoTitle: "Create PDF Files in C# | C# Generate PDF with Text, Image, Table, Forms"
description: "Use C# PDF API to create PDF files from scratch using C#. Add text, images, tables, and forms in PDF documents dynamically using C# or VB.NET."
date: Wed, 02 Dec 2020 22:49:24 +0000
draft: false
url: /2020/12/02/create-pdf-files-using-csharp/
author: Usman Aziz
summary: 'Automated generation and processing of [PDF][1] documents have become a demanding feature in recent days. In various applications, PDF documents are generated dynamically such as invoices, receipts, and different types of reports. In accordance with that, this article covers the basic implementation of PDF automation within .NET applications. Ultimately, you will learn **how to create PDF files and insert text, images, tables, and other components using C#**.'
tags: ['add forms in pdf in csharp', 'add table in pdf in csharp', 'add text in pdf in csharp', 'create pdf in csharp', 'edit pdf file in csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-PDF-Documents-using-C.jpg" alt="Create PDF Documents using C#">}}


Automated generation and processing of [PDF][2] documents have become a demanding feature in recent days. In various applications, PDF documents are generated dynamically such as invoices, receipts, and different types of reports. In accordance with that, this article covers the basic implementation of PDF automation within .NET applications. Ultimately, you will learn **how to create PDF files using C#**. The code samples will demonstrate **how to insert text, images, tables, and other components in PDF using C#**.

*   [C# PDF API - Free Download][3]
*   [Create PDF Files in C#][4]
*   [Edit Existing PDF in C#][5]
*   [Insert Image in PDF using C#][6]
*   [Create a Table in PDF using C#][7]
*   [Create a Form in PDF in C#][8]

**Info**: Aspose provides a free online web app that allows you to [view PDFs online][9], another that allows you to [convert PDFs to video][10], and one that allows you to [edit PDFs online][11].

## C# .NET PDF API - Free Download {#CSharp-PDF-API-Free-Download}

[Aspose.PDF for .NET][12] is a PDF file manipulation API that lets you generate and process PDF files from within your .NET applications. Using the API you can generate various kinds of reports and business documents dynamically. The API is available as a [downloadable DLL][13] as well as hosted on [NuGet][14].

```
Install-Package Aspose.Pdf
```

## Create PDF Files in C# {#Create-PDF-Files-in-CSharp}

Let's start by creating a simple PDF document containing a text fragment. The following are the steps to create a PDF file using C#.

*   Create an object of [Document][15] class.
*   Add a page to the document using [Document.Pages.Add()][16] method.
*   Create a new [TextFragment][17] object and set its text.
*   Add _TextFragment_ to the [Paragraphs][18] collection of the page.
*   Save the PDF file using [Document.Save(String)][19] method.

The following code sample shows how to create a simple PDF file using C#.

{{< gist aspose-com-gists af1939800a08a83bf57917e31b5f3b58 "create-pdf.cs" >}}

Read more about [creating complex PDF documents][20].

## Edit a PDF File in C# {#Edit-Existing-PDF-in-CSharp}

Modifying a PDF file is as simple as creating a new one. Simply load the file using the [Document][21] class, perform your desired operations, and save it. The following are the steps to modify a PDF.

*   Create an object of the [Document][22] class and provide a PDF file's path to its constructor.
*   Manipulate the pages or content of the document.
*   Save the document using [Document.Save()][23] method.

The following code sample shows how to modify a PDF using C#.

{{< gist aspose-com-gists af1939800a08a83bf57917e31b5f3b58 "edit-pdf.cs" >}}

## Insert Image in PDF using C# {#Insert-Image-in-PDF-using-CSharp}

Let's now check how to insert an image into the PDF document. The following are the steps to do so.

*   Create an object of [Document][24] class to open a PDF document.
*   Access the page you want to add an image to using [Page][25] class.
*   Add the image to the page’s [Resources][26] collection.
*   Use operators to place the image on the page:
    *   [GSave][27] operator to save the current graphical state.
    *   [ConcatenateMatrix][28] operator to specify where the image is to be placed.
    *   [Do][29] operator to draw the image on the page.
    *   Finally, use the [GRestore][30] operator to save the updated graphical state.
*   Save the PDF file.

The following code sample shows how to add an image to a PDF document using C#.

{{< gist aspose-com-gists af1939800a08a83bf57917e31b5f3b58 "insert-image.cs" >}}

Read more about [insert images in PDF][31].

## Create a Table in PDF using C# {#Create-a-Table-in-PDF-using-CSharp}

The tables are an essential component of the documents that are used to organize the data in the form of rows and columns. Aspose.PDF for .NET provides you with quite a simple way to create and insert tables in PDF documents. The following are the steps to perform this operation.

*   Load the PDF file using [Document][32] class.
*   Initialize a table and set its columns and rows using [Table][33] class.
*   Set table's settings (i.e. borders).
*   Populate table by creating rows using [Table.Rows.Add()][34] method.
*   Add the table to the page using _Document.Pages\[1\].Paragraphs.Add(Table)_ method.
*   Save the PDF file.

The following code sample shows how to create and add a table in a PDF document in C#.

{{< gist aspose-com-gists af1939800a08a83bf57917e31b5f3b58 "insert-table.cs" >}}

Read more about [creating tables in PDF][35].

## Create a Form in PDF in C# {#Create-a-Form-in-PDF-in-CSharp}

Forms in PDFs are used to collect the data from the readers. You can insert textboxes, checkboxes, radio buttons, and other supported controls in PDF forms. PDF format supports two types of forms; Acro forms and XFA forms ([see details][36]. The following are the steps to create and add forms in a PDF.

*   Load the PDF file using [Document][37] class.
*   Create form controls such as [TextBoxField][38].
*   Add control to the form using [Document.Form.Add(textBoxField, 1)][39] method.
*   Save the PDF document.

The following code sample shows how to add forms to the PDF document using C#.

{{< gist aspose-com-gists af1939800a08a83bf57917e31b5f3b58 "create-form.cs" >}}

Read more about [creating forms in PDF][40].

## Conclusion

In this post, you have learned how to create PDF files from scratch using C#. Furthermore, you have come to know how to insert various types of components such as text, images, tables, and forms in a PDF document programmatically. You can learn more about the PDF API using the [documentation][41].

## See Also

*   [Convert PDF to DOCX using C#][42]
*   [Add Text to a PDF Document using C#][43]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #CSharp-PDF-API-Free-Download
[4]: #Create-PDF-Files-in-CSharp
[5]: #Edit-Existing-PDF-in-CSharp
[6]: #Insert-Image-in-PDF-using-CSharp
[7]: #Create-a-Table-in-PDF-using-CSharp
[8]: #Create-a-Form-in-PDF-in-CSharp
[9]: https://products.aspose.app/slides/viewer/pdf
[10]: https://products.aspose.app/slides/video/pdf
[11]: https://products.aspose.app/slides/editor/pdf
[12]: https://products.aspose.com/pdf/net
[13]: https://downloads.aspose.com/pdf/net
[14]: http://nuget.org/packages/Aspose.pdf
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/pagecollection/methods/add
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[20]: https://docs.aspose.com/pdf/net/complex-pdf/
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/methods/save
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/resources
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/gsave
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/concatenatematrix
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/do
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/grestore
[31]: https://docs.aspose.com/pdf/net/working-with-images-in-pdf/
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf/rows/methods/add
[35]: https://docs.aspose.com/pdf/net/working-with-tables/
[36]: https://blog.aspose.com/2020/03/31/acroforms-vs-xfa-forms-convert-xfa-to-acroforms-in-pdf/)
[37]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[38]: https://apireference.aspose.com/pdf/net/aspose.pdf.forms/textboxfield
[39]: https://apireference.aspose.com/pdf/net/aspose.pdf.forms.form/add/methods/1
[40]: https://docs.aspose.com/pdf/net/working-with-forms/
[41]: https://docs.aspose.com/pdf/net/overview/
[42]: https://blog.aspose.com/2019/11/24/convert-pdf-to-word-doc-docx-in-csharp-vb-net/
[43]: https://blog.aspose.com/2021/08/26/add-text-to-a-pdf-using-csharp/





