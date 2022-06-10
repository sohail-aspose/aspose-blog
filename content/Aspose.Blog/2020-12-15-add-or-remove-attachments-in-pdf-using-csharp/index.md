---
title: 'Add and Remove Attachments in PDF using C#'
seoTitle: "C# Add or Remove Attachments in PDF | Extract PDF Attachments C#"
description: "Extract, add or remove attachments in PDF files using C#. Step by step guide with code samples to manipulate the PDF attachments programmatically."
date: Tue, 15 Dec 2020 18:22:35 +0000
draft: false
url: /2020/12/15/add-or-remove-attachments-in-pdf-using-csharp/
author: Usman Aziz
summary: 'The [PDF][1] format supports adding attachments to a PDF file similar to the email attachments. A PDF attachment could be of TXT, DOCX, XLSX, or any other document format. In this article, you will learn how to implement some basic PDF attachment manipulation features in your .NET applications. By the end of this article, you will be able to **extract, add, or remove attachments in a PDF programmatically using C#**.'
tags: ['add attachment in PDF csharp', 'extract attachment in PDF csharp', 'manipulate PDF attachments in csharp', 'remove attachment in PDF csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/add-remove-attachments-in-pdf-using-C.jpg" alt="add remove attachment in PDF in C#">}}


The [PDF][2] format supports adding attachments to a PDF file similar to the email attachments. A PDF attachment could be of TXT, DOCX, XLSX, or any other document format. In this article, you will learn how to implement some basic PDF attachment manipulation features in your .NET applications. By the end of this article, you will be able to **extract, add, or remove attachments in a PDF programmatically using C#**.

*   [PDF Attachment Manipulation API - Free Download][3]
*   [Add Attachments to PDF using C#][4]
*   [Extract PDF Attachment using C#][5]
*   [Remove Attachments from PDF using C#][6]

## PDF Attachment Manipulation API - Free Download {#PDF-Attachment-Manipulation-API}

[Aspose.PDF for .NET][7] is a well-known PDF manipulation API that lets you process PDF files seamlessly. You can read, create, edit, and convert the PDF files and manipulate the PDF attachments within a few steps. The API can be [downloaded][8] as DLL or MSI as well as installed using [NuGet][9].

```
Install-Package Aspose.Pdf
```

## Add Attachments to PDF using C# {#Add-Attachments-to-PDF-using-CSharp}

Aspose.PDF for .NET also allows you to add the attachments to a PDF file. For this, you simply need to add the file to [Document.EmbeddedFiles][10] collection using the [FileSpecification][11] class. The following are the steps to add an attachment to a PDF document.

*   Create a new PDF document using [Document][12] class.
*   Create an instance of [FileSpecification][13] class to load the attachment file.
*   Use [Document.EmbeddedFiles.Add(FileSpecification)][14] method to add the attachment.
*   Save the document using [Document.Save(String)][15] method.

The following code sample shows how to add an attachment to a PDF document using C#.

{{< gist aspose-com-gists d302a910cb473ea5b0c2ba72f777b13c "add-attachment.cs" >}}

## Extract PDF Attachment using C# {#Extract-PDF-Attachment-using-CSharp}

First of all, let's check out how to retrieve attachments from a PDF document. For this, follow the below steps:

*   Create an instance of the [Document][16] class.
*   Get the attachments into an [EmbeddedFileCollection][17] object using [Document.EmbeddedFiles][18] property.
*   Loop through attachments in the [EmbeddedFileCollection][19] using [FileSpecification][20] object.
*   Access properties of each attachment using [FileSpecification][21] object.
*   Save the attachment as a file (if required).

The following code sample shows how to extract PDF attachments using C#.

{{< gist aspose-com-gists d302a910cb473ea5b0c2ba72f777b13c "get-attachment.cs" >}}

## Remove Attachments from PDF using C# {#Remove-Attachments-from-PDF-using-CSharp}

You can either remove all or a particular attachment from a PDF file. For this, Aspose.PDF for .NET provides the following methods:

*   [Delete()][22] - Deletes all the attachments.
*   [Delete(String fileName)][23] - Deletes attachment by name.
*   [DeleteByKey(String Key)][24] - Deletes attachment by key in the collection.

The following are the steps to delete attachments from a PDF.

*   Create an instance of the [Document][25] class to load the PDF file.
*   Use [Document.EmbeddedFiles.Delete()][26] (or other delete method) to delete attachments.
*   Save the file using [Document.Save(String)][27] method.

The following code sample shows how to remove attachments from a PDF file in C#.

{{< gist aspose-com-gists d302a910cb473ea5b0c2ba72f777b13c "remove-attachment.cs" >}}

## Conclusion

In this article, you have seen how to manipulate the attachments in PDF documents programmatically. The step by step guide, API references, and code samples have shown how to retrieve, add, and remove attachments in PDF files using C#. You can learn more about Aspose.PDF for .NET using the [documentation][28].

## See Also

*   [Create PDF Files using C# – .NET PDF API][29]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #PDF-Attachment-Manipulation-API
[4]: #Add-Attachments-to-PDF-using-CSharp
[5]: #Extract-PDF-Attachment-using-CSharp
[6]: #Remove-Attachments-from-PDF-using-CSharp
[7]: https://products.aspose.com/pdf/net
[8]: https://downloads.aspose.com/pdf/net
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/embeddedfiles
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/filespecification
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/filespecification
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection/methods/add
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/embeddedfiles
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/filespecification
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/filespecification
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection/methods/delete
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.embeddedfilecollection/delete/methods/1
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection/methods/deletebykey
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/embeddedfilecollection/methods/delete
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[28]: https://docs.aspose.com/pdf/net/overview/
[29]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/





