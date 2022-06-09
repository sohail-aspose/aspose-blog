---
title: 'Create PDF File from Images using C#'
seoTitle: "Create PDF File from Images using C# | Image to PDF in C#"
description: "Use .NET PDF API to create PDF files from images using C#. Insert each image on a separate page in the PDF document programmatically."
date: Tue, 20 Apr 2021 11:41:00 +0000
draft: false
url: /2021/04/20/create-pdf-from-images-using-csharp/
author: Usman Aziz
summary: 'In different cases, you may need to create a PDF based on a bunch of images, such as generating PDF from scanned document pages or invoices. For such scenarios, this article covers **how to create PDF from the images programmatically using C#**.'
tags: ['Create PDF from Images using CSharp', 'Csharp API to Create PDF from Images', 'NET PDF API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-PDF-from-Images.jpg" alt="Create PDF from Images in C#">}}


In different cases, you may need to create a [PDF][1] based on a bunch of images, such as generating PDF from scanned document pages or invoices. For such scenarios, this article covers **how to create PDF from the images programmatically using [C#][2]**.

*   [API to Create PDF from Images][3]
*   [Steps to Generate a PDF File from Images][4]
*   [Create PDF from Images using C#][5]
*   [Get a Free API License][6]

## C# API to Create PDF from Images {#API-to-Generate-PDF-from-Images}

For creating the PDF files from images, we'll use [Aspsoe.PDF for .NET][7]. It is a powerful PDF API that lets you create, modify, and convert PDF files from within your .NET applications. You can either [download][8] the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.Pdf
```

## Steps to Create a PDF File from Images {#Steps-to-Generate-a-PDF-File-from-Image}

The following are the steps to create PDF from the images using Aspose.PDF for .NET.

*   First, create a new PDF document.
*   Get the list of the image files' names in an array.
*   For each image in the list, do the following:
    *   Add a new page to the PDF document and set its properties.
    *   Load each image file from the list.
    *   Add image to the paragraph collection of the page.
*   Finally, save the PDF document.

## Create PDF from Images using C# {#Generate-PDF-from-Images-using-Java}

The following are the steps along with API references to create PDF from images.

*   Create an instance of [Document][10] class.
*   Get the list of the image files' names in an array using [Directory.GetFiles(string)][11] method.
*   For each image file in the list, do the following:
    *   Add a new [Page][12] to the PDF document using [Document.Pages.Add()][13] method and set page’s properties.
    *   Load the image file into a [FileStream][14] object.
    *   Add a new [Image][15] to the page using [Page.Paragraphs.Add(Image)][16] method.
    *   Set image’s stream using [Image.ImageStream][17] property.
*   Finally, save the PDF document using [Document.Save(String)][18] method.

The following code sample shows how to create a PDF from images.

{{< gist aspose-com-gists 35546b3fb8da73ef8056e68a4d6caf97 "create-pdf-from-images.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the API without evaluation limitations by [getting a free temporary license][19].

## Conclusion

In this article, you have learned how to create PDF files from images using C#. The step-by-step guide and code sample have shown how to insert each image in a folder to a page in a PDF file. You can explore more about Aspose.PDF for .NET using [documentation][20]. In case you would have any queries, feel free to let us know via our [forum][21].

## See Also

*   [Generate PDF Files using C# – .NET PDF API][22]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/cs/
[3]: #API-to-Generate-PDF-from-Images
[4]: #Steps-to-Generate-a-PDF-File-from-Image
[5]: #Generate-PDF-from-Images-using-Java
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/pdf/net
[8]: https://downloads.aspose.com/pdf/net
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.directory.getfiles?view=net-5.0#System_IO_Directory_GetFiles_System_String_
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/pagecollection/methods/add
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/image
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/image/properties/imagestream
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/pdf/net/overview/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/





