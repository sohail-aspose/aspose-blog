---
title: 'Replace Images in PDF Files in C# .NET'
date: Wed, 18 May 2022 11:49:00 +0000
draft: false
url: /2022/05/18/replace-images-in-pdf-files-in-csharp-net/
author: 'Usman Aziz'
summary: '[PDF](https://docs.fileformat.com/pdf/) format is widely adopted to automatically generate the documents such as invoices, reports, articles, etc. In certain cases, you have to replace the images in the PDF documents, such as to hide the confidential content. To accomplish that programmatically, this article covers **how to replace images in PDF documents in C# .NET**.'
tags: ['DotNet API to Replace Images in PDF Files', 'DotNet PDF Generator API', 'Replace Images in a PDF File in CSharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Replace Images in PDF Files in C# .NET">}}


[PDF](https://docs.fileformat.com/pdf/) format is widely adopted to automatically generate the documents such as invoices, reports, articles, etc. In certain cases, you have to replace the images in the PDF documents, such as to hide the confidential content. To accomplish that programmatically, this article covers **how to replace images in PDF documents in C# .NET**.

*   [.NET API to Replace Images in PDF Files](#API-to-Replace-Images-in-PDF-Files)
*   [Replace Images in a PDF File](#Replace-Images-in-a-PDF-File)

## C# .NET API to Replace Images in PDF Files {#API-to-Replace-Images-in-PDF-Files}

To replace images in PDF files, we will use [Aspose.PDF for .NET](https://products.aspose.com/pdf/net/). The API is designed to perform PDF generation and manipulation from within the .NET applications. It allows you to create PDF documents of simple as well as complex layouts seamlessly. You can either [download](https://downloads.aspose.com/pdf/net/) the API's binaries or install it using [NuGet](http://nuget.org/packages/Aspose.PDF).

```
PM> Install-Package Aspose.PDF
```

## Replace Images in a PDF File in C# {#Replace-Images-in-a-PDF-File}

In PDF documents, the images are kept in an image collection of each page. Thus, you can access any of the images from the collection using its index and manipulate it. The following are the steps to replace a particular image in a PDF in C#.

*   Load the PDF file using [Document](https://apireference.aspose.com/pdf/net/aspose.pdf/document) class.
*   Get reference of the desired page from the PDF using [Document.Pages](https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages) collection.
*   Replace the image in the collection using [Pages\[index\].Resources.Images.Replace(imageIndex, new FileStream("lovely.jpg", FileMode.Open))](https://apireference.aspose.com/pdf/net/aspose.pdf/ximagecollection/methods/replace) method.
*   Save the updated document using [Document.Save(string)](https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5) method.

The following code sample shows how to replace an image in a PDF using C# .NET.

{{< gist aspose-com-gists a759c83d7c6bebb7142532b071e455b4 "replace-image-in-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license](https://purchase.aspose.com/temporary-license) in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to replace images in PDF files using C#. You can simply integrate the provided code sample and replace PDF images from within your applications. Besides, you can explore more about the C# PDF API using the [documentation](https://docs.aspose.com/pdf/net/). In case you would have any questions or queries, you can contact us via our [forum](https://forum.aspose.com/).

## See Also

*   [Add or Remove Annotations in PDF Files using C#](https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/)
*   [Extract Images from PDF using C#](https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/)
*   [Create PDF File from Images using C#](https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/)




