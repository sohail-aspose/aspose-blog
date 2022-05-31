---
title: 'Generate Thumbnails for PDF Files in C#'
date: Mon, 16 May 2022 05:45:00 +0000
draft: false
url: /2022/05/16/generate-thumbnails-for-pdf-files-in-csharp/
author: ''Usman Aziz''
summary: 'You may often need to generate thumbnails while embedding the [PDF][1] documents into a web application. Also, thumbnails of pages are required when creating a PDF viewer. For such scenarios, this article covers **how to generate thumbnails of a PDF file programmatically in C# .NET**. We will explicitly cover how to create a thumbnail of a particular page or all the pages in a PDF file.'
tags: ['DotNeT API to Generate Thumbnails of PDF', 'DotNet PDF Generator API', 'Generate Thumbnails of all Pages in PDF in CSharp', 'Generate a Thumbnail of a PDF File in CSharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Generate Thumbnails for PDF Files in C#">}}


You may often need to generate thumbnails while embedding the [PDF][2] documents into a web application. Also, thumbnails of pages are required when creating a PDF viewer. For such scenarios, this article covers **how to generate thumbnails of a PDF file programmatically in C# .NET**. We will explicitly cover how to create a thumbnail of a particular page or all the pages in a PDF file.

*   [.NET API to Generate Thumbnails of PDF][3]
*   [Generate a Thumbnail of a PDF File][4]
*   [Generate Thumbnails of all Pages in PDF][5]

## C# .NET API to Generate Thumbnails of PDF {#API-to-Generate-Thumbnails-of-PDF}

[Aspose.PDF for .NET][6] is a C# class library that lets you create and manipulate PDF documents within the .NET applications. Using the API, you can perform basic as well as advanced PDF automation operations quite easily. We will use this API to generate thumbnails of a PDF file. The API can be downloaded as [DLL][7] or installed via [NuGet][8].

```
PM> Install-Package Aspose.Pdf
```

## Generate a Thumbnail of a PDF File in C# .NET {#Generate-a-Thumbnail-of-a-PDF-File}

Usually, you have to generate a single thumbnail image for a PDF document. The page for thumbnail could be the cover page or any other page of your choice. The following are the steps to generate a thumbnail of the desired page of a PDF in C#.

*   Load the PDF file using the [Document][9] class.
*   Get a reference of the desired page from the [Document.Pages][10] collection.
*   Create a new [FileStream][11] for the image file.
*   Create an instance of the [Resolution][12] class to set the resolution of the thumbnail image.
*   Instantiate [JpegDevice][13] and set the height, width, resolution, and quality of the image.
*   Generate thumbnail using [JpegDevice.Process(Page, FileStream)][14] method.
*   Close the file stream.

The following code sample shows how to generate a thumbnail of a PDF file in C#.

{{< gist aspose-com-gists 3c70ee281bd9461139425323267f864b "generate-pdf-thumbnail.cs" >}}

## Generate Thumbnails of all Pages in PDF in C# {#Generate-Thumbnails-of-all-Pages-in-PDF}

The following are the steps to generate thumbnails for all the pages in PDF in C#.

*   Load the PDF file using the [Document][15] class.
*   Loop through all the pages in PDF using [Document.Pages][16] collection.
*   In each iteration, perform the following operations:
    *   Create a new [FileStream][17] for the image file.
    *   Create an instance of the [Resolution][18] class to set the resolution of the thumbnail image.
    *   Instantiate [JpegDevice][19] and set the height, width, resolution, and quality of the image.
    *   Generate thumbnail using [JpegDevice.Process(Page, FileStream)][20] method.
    *   Close the file stream.

The following code sample shows how to generate thumbnails for all the pages in PDF.

{{< gist aspose-com-gists 3c70ee281bd9461139425323267f864b "generate-pdf-thumbnail-all-pages.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][21] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to generate thumbnails for PDF files in C#. You have seen how to generate a thumbnail of a particular page or all the pages in a PDF file. Besides, you can explore more about the C# PDF API using the [documentation][22]. In case you would have any questions or queries, you can contact us via our [forum][23].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][24]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Generate-Thumbnails-of-PDF
[4]: #Generate-a-Thumbnail-of-a-PDF-File
[5]: #Generate-Thumbnails-of-all-Pages-in-PDF
[6]: https://products.aspose.com/pdf/net/
[7]: https://products.aspose.com/pdf/net/
[8]: http://nuget.org/packages/Aspose.PDF
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/resolution
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/jpegdevice
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/jpegdevice/methods/process
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[17]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/resolution
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/jpegdevice
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/jpegdevice/methods/process
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/pdf/net/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/




