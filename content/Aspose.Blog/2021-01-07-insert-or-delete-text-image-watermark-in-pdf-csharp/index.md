---
title: 'Insert or Delete Text/Image Watermark in PDF File using C#'
seoTitle: "Insert or Delete Text/Image Watermark in PDF File using C#"
description: "Insert or Delete Watermark in PDF document. Add or remove Image/Picture or Text watermark from PDF files programmatically using C#."
date: Thu, 07 Jan 2021 09:15:00 +0000
draft: false
url: /2021/01/07/insert-or-delete-text-image-watermark-in-pdf-csharp/
author: Farhan Raza
summary: 'Watermarks are frequently used in PDF files. You can **insert or delete text and image watermark in PDF** files with few simple steps. You can easily control a lot of properties for working with watermarks. For example, opacity, position, rotation, color, font, image, etc., and much more. Likewise, a lot of other properties can be set for watermarks with quick API calls.'
tags: ['Add watermark in PDF with C#', 'Delete watermrk from PDF with C#', 'Image watermark in PDF', 'Textual watermark in PDF', 'Visual watermark in PDF', 'delete watermark from PDF', 'insert image watermark in PDF', 'insert text watermark in PDF', 'insert watermark in PDF', 'remove watermark from PDF']
categories: ['Aspose.PDF Product Family']
---

Watermarks are frequently used in [PDF][1] files. You can insert or delete text and image watermark in PDF files with few simple steps. You can easily control a lot of properties for working with watermarks. For example, opacity, position, rotation, color, font, image, etc., and much more. Likewise, a lot of other properties can be set for watermarks with quick API calls. Let us explore this topic further by walking through the following sections:

*   [Add or Delete Image/Text Watermark in PDF – API Installation][2]
*   [Insert Text Watermark in PDF File Programmatically using C#][3]
*   [Insert Image Watermark in PDF File Programmatically using C#][4]
*   [Delete Image or Text Watermark in PDF File using C#][5]

## Add or Delete Image/Text Watermark in PDF – API Installation {#section1}

[Aspose.PDF for .NET][6] API lets you create, edit, and manipulate your PDF documents. You can easily work with the feature of adding or deleting watermarks in PDF documents. You can download the latest DLL files from the [New Releases][7] section, or install them with the following [NuGet][8] command:

```
PM> Install-Package Aspose.Pdf
```

The API will be configured within a couple of minutes and now you are all set to work with watermarks in PDF documents.

## Insert Text Watermark in PDF File Programmatically using C# {#section2}

Text watermarks are frequently used in PDF documents to show the purpose or nature of the document. For example, some organization may add a text watermark as “Classified” or “Confidential” based on the nature of the document. Likewise, you can control the font size, font style, color, rotation, position, etc. You can add a text watermark in PDF file with the following steps:

1.  Load input PDF document
2.  Create [TextStamp][9] class instance
3.  Set origin and other properties
4.  Set [Stamp ID][10] for text watermark to later identify it
5.  Add a stamp to a particular page
6.  Save output PDF with text watermark

The following code snippet explains how to add or insert text watermark in PDF file using C#:

{{< gist aspose-com-gists 3af3aa36eb0b98453aee3b39ab6348f6 "Add_Text_Watermark.cs" >}}

## Insert Image Watermark in PDF File Programmatically using C# {#section3}

Images contain a lot of meaningful information so the image watermarks are also frequently used in PDF files. For example, a document issued from some organization or institute may have its logo in the background of the page. You can work with the feature of inserting image watermark in PDF documents using [C#][11] with the steps below:

1.  Load input PDF document
2.  Access any page of the input PDF
3.  Create [image stamp][12]
4.  Center adjust the image watermark based on page dimensions
5.  Set stamp id for deleting the watermark later, if required
6.  Add a stamp to particular page OR on all pages
7.  Save output PDF with image watermark

The code snippet below shows how to insert image watermark in PDF file with C#:

{{< gist aspose-com-gists 3af3aa36eb0b98453aee3b39ab6348f6 "Add_Image_Watermark.cs" >}}

You can notice the centrally aligned image watermark of the PDF file in the screenshot:



{{< figure align=center src="images/Image_Watermark_PDF.png" alt="Image Watermark PDF">}}


## Delete Image or Text Watermark in PDF File using C# {#section4}

You can remove/delete a watermark from a PDF document. An image watermark or text watermark can be identified with a stamp id property which was set in above examples while adding the watermarks. You need to follow the steps below to delete watermark from PDF file:

1.  Initialize [PdfContentEditor][13] class object
2.  Call [BindPdf][14] method
3.  Delete watermark using specific id
4.  Save output PDF with removed watermark

The code below shows how to delete image or text watermark from PDF file in C#:

{{< gist aspose-com-gists 3af3aa36eb0b98453aee3b39ab6348f6 "Remove_Watermark.cs" >}}

## Conclusion

In this article, you have learned how to insert image watermark or text watermark in a PDF document programmatically using C#. Likewise, we have also explored how to delete image or text watermark in PDF file using C# language in .NET based applications. Furthermore, in case of any further query or information, you can write to us at Free Support Forum.

## See Also

[Convert PDF File to Byte Array or Byte Array to PDF using C#][15]




[1]: https://docs.fileformat.com/pdf/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/pdf/net
[7]: https://downloads.aspose.com/pdf/net
[8]: https://www.nuget.org/packages/Aspose.Pdf
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/textstamp
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/stamp/methods/setstampid
[11]: https://docs.fileformat.com/programming/cs/
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/imagestamp
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfcontenteditor/fields/index
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades.pdfcontenteditor/bindpdf/methods/1
[15]: https://blog.aspose.com/2020/11/29/convert-file-byte-array-pdf-csharp/





