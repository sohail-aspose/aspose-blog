---
title: 'Rotate PDF Pages, the Text or Image with C# or VB.NET'
seoTitle: "Rotate PDF File Page | Rotate Text or Image in PDF with C# or VB.NET"
description: "Rotate PDF page. Rotate Specific, certain, particular pages or the text and image/picture using C# or VB.NET programmatically."
date: Sun, 18 Oct 2020 21:07:00 +0000
draft: false
url: /2020/10/18/rotate-pdf-text-image-page-with-csharp-vb-net/
author: Farhan Raza
summary: 'Let us explore how to rotate PDF pages as well as how to rotate text or images/pictures in a PDF document in your .NET applications. You can work with Aspose.PDF for .NET API to call the methods and APIs using C# or VB.NET languages.'
tags: ['pdf rotation', 'rotate PDF c#', 'rotate image in PDF C#', 'rotate pdf', 'rotate pdf pages', 'rotate text in PDF C#']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/rotate-pdf-image-text.png" alt="rotate pdf pages images text C#">}}


Let us explore the scenarios related to rotation in [PDF][1] documents. You can rotate whole pages or PDF page contents including text or images programmatically using C# or VB.NET in your applications. You will be walking through the following PDF pages, images, or text rotation scenarios with the help of simple and basic examples of PDF rotation features:

*   [PDF Rotation API – Installation][2]
*   [Rotate All pages of PDF Document using C#][3]
*   [Rotate Specific Pages of PDF using C#][4]
*   [Rotate Text on PDF Document using C#][5]
*   [Rotate Image on PDF using C#][6]

## PDF Rotation API – Installation {#section0}

You can efficiently achieve your PDF rotation requirements with [Aspose.PDF for .NET][7] API. You can integrate it in your .NET applications by downloading from the [Releases][8] section or via [NuGet][9] using the following installation command:

```
Install-Package Aspose.Pdf
```

Once the API is configured successfully, you can use the [Rotation][10] enumeration to select a suitable value of rotation in the clockwise direction.

## Rotate All Pages of PDF Document using C# {#section1}

Let us assume a PDF document created by scanning some documents where all images are scanned at specific angle. Like all pages are rendered upside down and you need to rotate all pages of PDF document in your C# or VB.NET application. Likewise, there could be thousands of related use cases where you need to rotate PDF files. You can rotate all pages of a PDF file with following steps:

1.  Load input PDF document
2.  Iterate through each page
3.  Rotate the pages of PDF with [Rotation][11] property
4.  Save output PDF file

The code snippet below shows how to rotate all pages of a PDF file with C# or VB.NET:

{{< gist aspose-com-gists e9637e99932cbbf4f82455094769173b "Rotate-All-Pages.cs" >}}

## Rotate Specific Pages of PDF with C# {#section2}

The rotation in a PDF document is applied on page level. Therefore, you can also rotate specific pages of PDF file as per your requirements. You only need to choose the page number you want to apply the rotation on. The steps below explain how to rotate certain pages of PDF file:

1.  Load input PDF document
2.  Specify the page numbers to be rotated
3.  Iterate through certain page numbers
4.  Rotate the pages at particular angle
5.  Save output PDF file

The following code snippet elaborates how to rotate specific or certain pages in a PDF document using C# or VB.NET:

{{< gist aspose-com-gists e9637e99932cbbf4f82455094769173b "Rotate-Specific-Pages.cs" >}}

## Rotate Text on PDF Document using C# {#section3}

While adding text in PDF documents, you can rotate text at different angles. This text rotation can be more relevant while adding some watermark text in PDF document. Let us add some text at specific coordinates on page and rotate the text diagonally on 45 degrees.

1.  Initialize object of [Document][12] class
2.  Add a blank page to the PDF document
3.  Create new [TextFragment][13] object
4.  Add text at specific coordinates of the page
5.  [Append][14] Text and Save the output PDF file

The code snippet below shows how to rotate text in PDF document using C# or VB.NET:

{{< gist aspose-com-gists e9637e99932cbbf4f82455094769173b "Rotated-Text.cs" >}}

## Rotate Image on PDF using C# {#section4}

You can rotate image in a PDF document while adding or inserting the image in the PDF file. It can be helpful when you want to update or change the orientation of the image. You can follow these steps to rotate image on a PDF page:

1.  Load input PDF document
2.  Create an instance of [ImageStamp][15] class
3.  Set different properties including rotation
4.  Save output PDF file

The following code demonstrates how to rotate image or picture in a PDF document programmatically using C# or VB.NET:

{{< gist aspose-com-gists e9637e99932cbbf4f82455094769173b "Rotate-Image.cs" >}}

## Conclusion

In this article, you have explored how to rotate PDF pages as well as how to rotate text or images/pictures in a PDF document in your .NET applications. You can work with Aspose.PDF for .NET API to call the methods and APIs using C# or VB.NET languages. Moreover, you can reach us at [Free Support Forum][16] if you want to discuss any related scenario with us. We will be pleased to guide you!

## See Also

[Compress, or Optimize PDF Files with Same Quality using Java][17]




[1]: https://docs.fileformat.com/pdf/
[2]: #section0
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: https://products.aspose.com/pdf/net
[8]: https://releases.aspose.com/
[9]: https://www.nuget.org/packages/Aspose.Pdf
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/rotation
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/rotation
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder/methods/appendtext
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/imagestamp
[16]: https://forum.aspose.com/c/pdf
[17]: https://blog.aspose.com/2020/10/14/compress-optimize-reduce-pdf-file-size-with-same-quality-java/





