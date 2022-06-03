---
title: 'Convert OneNote Document to PDF using C#'
date: Thu, 12 May 2022 06:27:20 +0000
draft: false
url: /2022/05/12/convert-onenote-document-to-pdf-using-csharp/
author: 'Muzammil Khan'
summary: 'As a .NET developer, you can easily export notes from OneNote documents to PDF. In this article, you will learn **how to convert a OneNote document to a PDF using C#.**'
tags: ['Convert OneNote to PDF', 'Convert OneNote to PDF C#', 'OneNote to PDF', 'OneNote to PDF Converter', 'OneNote to PDF using C#', 'Save OneNote as PDF in C#']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/convert-onenote-document-to-pdf-using-csharp.jpg" alt="Convert OneNote Document to PDF using C#">}}


[OneNote][1] document is a digital notebook used to collect, organize, and collaborate free form information and multi-user collaboration in the form of notes, drawings, screen clippings, and audio commentaries. In certain cases, we may need to export the content of OneNote documents into PDF documents. [PDF][2] is the most popular format for sharing and printing documents without losing the formatting. In this article, we will learn **how to convert a OneNote document to a PDF using C#**.

The following topics shall be covered in this article:

*   [OneNote to PDF Converter C# API][3]
*   [Convert Existing OneNote Document to PDF][4]
*   [Create OneNote Document and Convert it to PDF][5]
*   [Convert Range of OneNote Pages to PDF][6]
*   [Convert OneNote to PDF with Image Compression][7]

## OneNote to PDF Converter C# API {#OneNote-to-PDF-Converter-CSharp-API}

For converting OneNote documents to PDF, we will be using the [Aspose.Note for .NET][8] API. It allows creating, reading, and converting OneNote documents programmatically without using Microsoft OneNote. Please either [download][9] the DLL of the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Note
```

## Convert Existing OneNote Document to PDF using C# {#Convert-Existing-OneNote-Document-to-PDF-using-CSharp}

We can convert an existing OneNote document to a PDF by following the steps given below:

1.  Load a OneNote file using the **_[Document][11]_** class.
2.  Call the **_[Save()][12]_** method to save the OneNote document as a PDF. It takes the output PDF file path and the Save Format as arguments.

The following code sample shows **how to convert an existing OneNote document to a PDF using C#**.

{{< gist aspose-com-gists 8dfea432c8157108ceb7f23d8733ec65 "Convert-OneNote-to-PDF-CSharp_Convert.cs" >}}



{{< figure align=center src="images/Convert-Existing-OneNote-Document-to-PDF-using-CSharp-1024x512.jpg" alt="Convert Existing OneNote Document to PDF using C#" caption="Convert Existing OneNote Document to PDF using C#.">}}


## Create OneNote Document and Convert to PDF using C# {#Create-OneNote-Document-and-Convert-to-PDF-using-CSharp}

We can create a OneNote document and convert it to a PDF programmatically by following the steps given below:

1.  Firstly, create an instance of the **_[Document][13]_** class.
2.  Next, create a new page using the [**_Page_**][14] class object.
3.  Then, add the newly created page to the document using the [**_AppendChildLast()_**][15] method.
4.  After that, add content such as Page Title, etc.
5.  Finally, call the **_[Save()][16]_** method to save the OneNote document as a PDF. It takes the output PDF file path as an argument.

The following code sample shows **how to create a OneNote document and convert it to a PDF using C#**.

{{< gist aspose-com-gists 8dfea432c8157108ceb7f23d8733ec65 "Convert-OneNote-to-PDF-CSharp_CreateAndConvert.cs" >}}

## Convert Range of OneNote Pages to PDF using C# {#Convert-Range-of-OneNote-Pages-to-PDF-using-CSharp}

We can convert a range of pages from a OneNote document to a PDF by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][17]_** class.
2.  Next, define **_[PdfSaveOptions][18]_** class object.
3.  Then, set the _**PageIndex **_from where to start the conversion.
4.  After that, set **_PageCount _**to convert a total number of pages.
5.  Finally, call the **_[Save()][19]_** method to save the OneNote document as a PDF. It takes the output PDF file path and **_PdfSaveOptions_** as arguments.

The following code sample shows **how to convert a range of pages from a OneNote document to a PDF using C#**.

{{< gist aspose-com-gists 8dfea432c8157108ceb7f23d8733ec65 "Convert-OneNote-to-PDF-CSharp_ConvertPages.cs" >}}

## Convert OneNote to PDF with Image Compression in C# {#Convert-OneNote-to-PDF-with-Image-Compression-in-CSharp}

We can compress images of a OneNote document while converting it to a PDF document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][20]_** class.
2.  Next, define **_[PdfSaveOptions][21]_** class object.
3.  Then, set the _**[ImageCompression][22]**_ type as JPEG.
4.  After that, set the quality for JPEG compression using the **_[JpegQuality][23]_**.
5.  Finally, call the **_[Save()][24]_** method to save the OneNote document as a PDF. It takes the output PDF file path and **_PdfSaveOptions_** as arguments.

The following code sample shows **how to convert a OneNote document to a PDF and apply image compression using C#**.

{{< gist aspose-com-gists 8dfea432c8157108ceb7f23d8733ec65 "Convert-OneNote-to-PDF-CSharp_ConvertWithImageCompression.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][25] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create a new OneNote document using C#;
*   save the OneNote document as a PDF programmatically;
*   export a OneNote document to PDF and compress images.

Besides, you can learn more about [Aspose.Note for .NET][26] API using the [documentation][27]. In case of any ambiguity, please feel free to contact us on the [forum][28].

## See Also

*   [Convert OneNote Document to HTML Webpage using C#][29]
*   [Convert OneNote .one to Word DOCX DOC File][30]
*   [Create OneNote Files and Add Images, Tables, and Tags to OneNote File using C#][31]




[1]: https://docs.fileformat.com/note-taking/one/
[2]: https://docs.fileformat.com/pdf/
[3]: #OneNote-to-PDF-Converter-CSharp-API
[4]: #Convert-Existing-OneNote-Document-to-PDF-using-CSharp
[5]: #Create-OneNote-Document-and-Convert-to-PDF-using-CSharp
[6]: #Convert-Range-of-OneNote-Pages-to-PDF-using-CSharp
[7]: #Convert-OneNote-to-PDF-with-Image-Compression-in-CSharp
[8]: https://products.aspose.com/note/net
[9]: https://downloads.aspose.com/note/net
[10]: https://www.nuget.org/packages/aspose.note
[11]: https://apireference.aspose.com/note/net/aspose.note/document
[12]: https://apireference.aspose.com/note/net/aspose.note.document/save/methods/4
[13]: https://apireference.aspose.com/note/net/aspose.note/document
[14]: https://apireference.aspose.com/note/net/aspose.note/page
[15]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/appendchildlast/_1
[16]: https://apireference.aspose.com/note/net/aspose.note.document/save/methods/3
[17]: https://apireference.aspose.com/note/net/aspose.note/document
[18]: https://apireference.aspose.com/note/net/aspose.note.saving/pdfsaveoptions
[19]: https://apireference.aspose.com/note/net/aspose.note.document/save/methods/3
[20]: https://apireference.aspose.com/note/net/aspose.note/document
[21]: https://apireference.aspose.com/note/net/aspose.note.saving/pdfsaveoptions
[22]: https://apireference.aspose.com/note/net/aspose.note.saving/pdfsaveoptions/properties/imagecompression
[23]: https://apireference.aspose.com/note/net/aspose.note.saving/pdfsaveoptions/properties/jpegquality
[24]: https://apireference.aspose.com/note/net/aspose.note.document/save/methods/5
[25]: https://purchase.aspose.com/temporary-license
[26]: https://products.aspose.com/note/
[27]: https://docs.aspose.com/note/net/
[28]: https://forum.aspose.com/c/note/28
[29]: https://blog.aspose.com/2022/04/16/convert-onenote-document-to-html-webpage-using-csharp/
[30]: https://blog.aspose.com/2021/09/01/convert-onenote-file-.one-to-word-document-docx-or-doc/
[31]: https://blog.aspose.com/2020/05/08/create-onenote-files-add-images-tables-tags-to-onenote-file-using-csharp/




