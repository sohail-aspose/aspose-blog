---
title: 'Convert PDF File to PowerPoint Presentation in C#'
seoTitle: ""
description: ""
date: Wed, 18 Mar 2020 13:15:29 +0000
draft: false
url: /2020/03/18/convert-pdf-to-powerpoint-ppt-pptx-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Convert PDF to PPT', 'Convert PDF to PPTX', 'PDF to PPT in Csharp', 'PDF to PPTX in CSharp', 'PDF to PowerPoint']
categories: ['Aspose.PDF Product Family']
---

This article contains the steps and code samples to **convert PDF to PPT or PPTX** programmatically in **C#**.



{{< figure align=center src="images/Convert-PDF-to-PPT-C.png" alt="Convert PDF to PPT C#">}}


PDF is one of the widely used formats for exchanging documents with reliability without worrying about layout issues. The PowerPoint presentations (PPT/PPTX), on the other hand, have made it easier to present the data or information in the form of interactive slides. In some cases, the information contained in a PDF file is needed to be presented as a PowerPoint presentation. For such a case, you can minimize the efforts by automating the process of importing information from PDF to PowerPoint PPT/PPTX.

In order to deal with the above-mentioned scenario, this article will demonstrate how to:

*   [Convert PDF to PowerPoint PPT or PPTX in C#.][1]
*   [Convert PDF to PowerPoint PPT or PPTX with slides as images in C#.][2]
*   [Track PDF to PowerPoint conversion progress.][3]

**Info**: Using its own APIs, Aspose developed a [free online service for converting PDF to PowerPoint.][4]

## C# API for PDF to PowerPoint Conversion

In order to convert PDF to PPT or PPTX, we'll use [Aspose.PDF for .NET][5] which is a powerful PDF API to create, process and convert PDF documents. _Aspose.PDF for .NET_ is available on [NuGet][6] as well as in the form of DLL in the [Downloads][7] section.

## Convert PDF to PPT or PPTX in C# {#Convert-PDF-to-PPT-or-PPTX-in-CSharp}

The following are the steps to convert a PDF file to a PowerPoint presentation using _Aspose.PDF for .NET_.

*   Create an object of the [Document][8] class.
*   Create an object of the [PptxSaveOptions][9] class.
*   Call the [Document.Save()][10] method to save the PDF as PPT or PPTX.

The following code sample shows how to convert PDF to PPT in C#.

{{< gist aspose-com-gists 40a0786267527e39582ec6fc8d23338e "convert-pdf-to-ppt.cs" >}}

### PDF Document



{{< figure align=center src="images/PDF-Document.png" alt="">}}


### Converted PowerPoint PPT



{{< figure align=center src="images/Convert-PDF-to-PPT-in-C.png" alt="">}}


## Convert PDF to PPT in C# - Rendering Slides as Images {#Rendering-Slides-as-Images}

In case you want to avoid having selectable text in the converted PowerPoint presentation, you can render each slide as an image. For this, you can set [PptxSaveOptions.SlidesAsImages][11] property to _true_ and the rest of the steps will remain the same.

The following code sample shows how to convert PDF to PPT having slides as images in C#.

{{< gist aspose-com-gists 40a0786267527e39582ec6fc8d23338e "convert-pdf-to-ppt-slide-images.cs" >}}

## Track PDF to PPT Conversion Progress {#Track-PDF-to-PPT-Conversion-Progress}

You may also track the progress of the PDF to PPT conversion process using _Aspose.PDF for .NET_. The following information can be retrieved about the conversion process:

*   Total progress of the conversion
*   End of analysis of each page before conversion
*   Creation of result page before physical export
*   Export of each result page

The following code sample shows how to track the PDF to PPT conversion in C#.

{{< gist aspose-com-gists 40a0786267527e39582ec6fc8d23338e "convert-pdf-to-ppt-track-progress.cs" >}}

### Output



{{< figure align=center src="images/Track-PDF-to-PPT-Progress-C.png" alt="">}}


## Related Articles

*   [Convert PDF to PowerPoint using Java][12]
*   [Convert PDF to Excel in C#][13]
*   [Convert PDF to Word in C#][14]




[1]: #Convert-PDF-to-PPT-or-PPTX-in-CSharp
[2]: #Rendering-Slides-as-Images
[3]: #Track-PDF-to-PPT-Conversion-Progress
[4]: https://products.aspose.app/slides/import/pdf-to-powerpoint
[5]: https://products.aspose.com/pdf/net
[6]: http://nuget.org/packages/aspose.pdf
[7]: https://downloads.aspose.com/pdf/net
[8]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[9]: https://apireference.aspose.com/net/pdf/aspose.pdf/pptxsaveoptions
[10]: https://apireference.aspose.com/net/pdf/aspose.pdf.document/save/methods/6
[11]: https://apireference.aspose.com/net/pdf/aspose.pdf/pptxsaveoptions/properties/slidesasimages
[12]: https://blog.aspose.com/2020/07/23/convert-pdf-to-powerpoint-ppt-pptx-using-java/
[13]: https://blog.aspose.com/2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/
[14]: https://blog.aspose.com/2019/11/24/convert-pdf-to-word-doc-docx-in-csharp-vb-net/





