---
title: 'Convert GIF Images to PDF in C#'
seoTitle: "Convert GIF to PDF in C# | Convert GIF Frames to PDF in C#"
description: "Use .NET image processing API to convert GIF images to PDF using C#. Convert all or the seletced frames in GIF to PDF using C#."
date: Tue, 09 Mar 2021 09:12:00 +0000
draft: false
url: /2021/03/09/convert-gif-images-to-pdf-in-csharp/
author: Usman Aziz
summary: 'PDF has become one of the ruling document formats nowadays. The cross-platform support has made PDF a universal format. Therefore, various documents or images are converted to PDF before they are shared or exchanged. In this article, you will learn **how to perform GIF to PDF conversion from within your C# applications**. The article will also cover how to customize GIF to PDF conversion in various cases.'
tags: ['Convert GIF to PDF using Csharp', 'Convert a Frame of GIF to PDF csharp', 'Set PDF Document Info in GIF to PDF Conversion csharp', 'Set Page Size in GIF to PDF Conversion csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/gif-to-pdf-icon.jpg" alt="gif to pdf c#">}}


[PDF][1] has become one of the ruling document formats nowadays. The cross-platform support has made PDF a universal format. Therefore, various documents or images are converted to PDF before they are shared or exchanged. In this article, you will learn **how to perform [GIF][2] to PDF conversion from within your C# applications**. The article will also cover how to customize GIF to PDF conversion in various cases.

*   [C# GIF to PDF Converter API][3]
*   [Convert GIF to PDF using C#][4]
*   [Convert Specific Frames of GIF to PDF][5]
*   [Set Page Size in GIF to PDF Conversion][6]
*   [Set PDF Document Info in GIF to PDF Conversion][7]
*   [Get a Free API License][8]

**Info**: Aspose recently developed a FREE [Text to GIF Converter][9].

## C# GIF to PDF Converter API {#GIF-to-PDF-Converter-API}

[Aspose.Imaging for .NET][10] is a feature-rich image processing API that lets you process and convert a wide range of image formats. Particularly, the API provides a high fidelity conversion of GIF images to PDF format. You can either [download][11] the API or install it using [NuGet][12].

```
PM> Install-Package Aspose.Imaging
```

## Convert GIF to PDF using C# {#Convert-GIF-to-PDF-using-csharp}

The following are the steps to convert a GIF image to PDF using Aspose.Imaging for .NET.

*   Use [Image][13] class to load the image.
*   Create an instance of [PdfOptions][14] class.
*   Convert GIF to PDF using [Image.Save(String, PdfOptions)][15] method.

The following code sample shows how to convert GIF to PDF using C#.

{{< gist aspose-com-gists dbe03a37114bd480493e67d6beb9d653 "gif-to-pdf.cs" >}}



{{< figure align=center src="images/gif-to-pdf.jpg" alt="GIF to PDF ">}}


## Convert Specific Frames of GIF to PDF in C# {#Convert-a-Frame-of-GIF-to-PDF}

You can also convert the specific frames from GIF to PDF. The following are the steps to perform this operation.

*   Use [Image][16] class to load the image.
*   Create an instance of [PdfOptions][17] class.
*   Use [PdfOptions.MultiPageOptions][18] property to set a range of pages.
*   Convert GIF to PDF using [Image.Save(String, PdfOptions)][19] method.

The following code sample shows how to convert specific frames of GIF to PDF using C#.

{{< gist aspose-com-gists dbe03a37114bd480493e67d6beb9d653 "gif-to-pdf-frame.cs" >}}

## Set Page Size in GIF to PDF Conversion {#Set-Page-Size-in-GIF-to-PDF-Conversion}

Aspose.Imaging for .NET also allows you to set the dimensions of the page in the converted PDF file. The following are the steps to perform this operation.

*   Use [Image][20] class to load the image.
*   Create an instance of [PdfOptions][21] class.
*   Use [PdfOptions.PageSize][22] property to set page size.
*   Convert GIF to PDF using [Image.Save(String, PdfOptions)][23] method.

The following code sample shows how to set page size in GIF to PDF conversion.

{{< gist aspose-com-gists dbe03a37114bd480493e67d6beb9d653 "gif-to-pdf-page-size.cs" >}}

## Set Document Info in GIF to PDF Conversion {#Set-PDF-Document-Info-in-GIF-to-PDF-Conversion}

PDF format supports setting additional information about a document such as author, keywords, subject, and title. Using Aspose.Imaging for .NET, you can set these properties in GIF to PDF conversion. The following are the steps to set document information for the converted PDF file.

*   Use [Image][24] class to load the image.
*   Create an instance of [PdfOptions][25] class.
*   Create an instance of [PdfDocumentInfo][26] class and set its properties.
*   Assign _PdfDocumentInfo_ object to [PdfOptions.PdfDocumentInfo][27] property.
*   Convert GIF to PDF using [Image.Save(String, PdfOptions)][28] method.

The following code sample shows how to set document information in GIF to PDF conversion using C#.

{{< gist aspose-com-gists dbe03a37114bd480493e67d6beb9d653 "gif-to-pdf-docinfo.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][29].

## Conclusion

In this article, you have learned how to convert GIF images to PDF documents using C#. Furthermore, you have seen how to convert specific frames of the GIF image and set page size or document information of converted PDF files. You can explore more about the C# image processing API using [documentation][30]. In case you would have any questions or queries, contact us via our [forum][31].

## See Also

*   [Compress PNG, JPEG, and TIFF Images using C#][32]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/image/gif/
[3]: #GIF-to-PDF-Converter-API
[4]: #Convert-GIF-to-PDF-using-csharp
[5]: #Convert-a-Frame-of-GIF-to-PDF
[6]: #Set-Page-Size-in-GIF-to-PDF-Conversion
[7]: #Set-PDF-Document-Info-in-GIF-to-PDF-Conversion
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.app/slides/text-to-gif
[10]: https://products.aspose.com/imaging/net
[11]: https://downloads.aspose.com/imaging/net
[12]: http://nuget.org/packages/Aspose.Imaging
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/imageoptionsbase/properties/multipageoptions
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions/properties/pagesize
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions
[26]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.pdf/pdfdocumentinfo
[27]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions/properties/pdfdocumentinfo
[28]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/imaging/net/getting-started/
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/





