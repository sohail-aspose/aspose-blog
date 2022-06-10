---
title: 'Convert CAD's DWG and DXF to PDF using C#'
seoTitle: "DWG DXF to PDF C# | Convert CAD Files to PDF in C# .NET"
description: "Use C# .NET CAD to PDF converter API to convert DWG or DXF to PDF using C#. DWG to PDF to DXF to PDF with customized rendering options."
date: Wed, 02 Sep 2020 16:33:29 +0000
draft: false
url: /2020/09/02/convert-autocad-dwg-dxf-to-pdf-using-csharp/
author: Usman Aziz
summary: '[AutoCAD][1] is used by designers to create various types of designs of buildings, bridges, automobiles, chips and etc. in a wide range of industries. However, the AutoCAD formats ([DWG][2], [DXF][3], etc.) can only be viewed in a dedicated software or an [online AutoCAD viewer][4]. To make things easier, the AutoCAD drawings could be converted into PDF files which can be viewed anywhere without any dependency. In this article, you will learn **how to convert AutoCAD DWG/DXF drawings to PDF programmatically using C#**.'
tags: ['convert autocad drawing to pdf', 'convert autocad layer to pdf csharp', 'convert autocad to pdf csharp', 'convert dwg to pdf csharp', 'convert dxf to pdf csharp']
categories: ['Aspose.CAD Product Family']
---

[CAD][5] is used by designers to create various types of designs of buildings, bridges, automobiles, chips and etc. in a wide range of industries. However, the CAD formats ([DWG][6], [DXF][7], etc.) can only be viewed in a dedicated software or an [online CAD viewer][8]. To make things easier, the DWG/DXF files could be converted into PDF files which can be viewed anywhere without any dependency. In this article, you will learn **how to convert CAD's DWG or DXF files to PDF using C#**.

*   [C# CAD to PDF Converter API][9]
*   [Convert DWG/DXF to PDF using C#][10]
*   [Set Canvas Size in DWG/DXF to PDF using C#][11]
*   [Perform Auto Scaling in CAD to PDF in C#][12]
*   [Modify Background and Drawing Color in PDF using C#][13]
*   [Convert Specific Layers of CAD to PDF using C#][14]

## C# CAD to PDF Converter - Free Download {#CSharp-AutoCAD-to-PDF-Converter-API}

[Aspose.CAD for .NET][15] is a powerful CAD to PDF converter API that lets you convert DWG and DXF files to PDF format quiet easily. In addition, it allows you to convert the CAD drawings to raster images. The API can be installed using the NuGet or downloaded as DLL from the [Downloads][16] section.

```
PM> Install-Package Aspose.CAD
```

## DWG or DXF to PDF C# Conversion {#Convert-AutoCAD-Drawing-to-PDF-using-CSharp}

The following are the steps to convert a DWG/DXF file to PDF format using Aspose.CAD for .NET API.

*   Load the AutoCAD DWG/DXF file using the [Image][17] class.
*   Create an object of [PdfOptions][18] class.
*   Save AutoCAD drawing as PDF using [Image.Save(String, ImageOptionsBase)][19] method.

The following code sample shows how to convert DWG to PDF using C#.

{{< gist aspose-com-gists e20eb36e47c431f229254444d9722fd0 "autocad-to-pdf.cs" >}}

## C# DWG/DXF to PDF - Set Canvas Size {#Set-Canvas-Size-in-AutoCAD-to-PDF-using-CSharp}

Aspose.CAD for .NET also allows you to specify the size of the pages (height and width) in the converted PDF document. The following are the steps to customize page size in CAD to PDF conversion.

*   Load the AutoCAD DWG/DXF file using the [Image][20] class.
*   Create an instance of [CadRasterizationOptions][21] class.
*   Set [CadRasterizationOptions.PageWidth][22] and [CadRasterizationOptions.PageHeight][23] properties.
*   Create an object of [PdfOptions][24] class.
*   Set [PdfOptions.VectorRasterizationOptions][25] property with _CadRasterizationOptions_ object.
*   Convert DWG or DXF to PDF using [Image.Save(String, ImageOptionsBase)][26] method.

The following code sample shows how to convert DXF to PDF using C#.

{{< gist aspose-com-gists e20eb36e47c431f229254444d9722fd0 "autocad-to-pdf-canvas-size.cs" >}}

## C# CAD to PDF - Auto Scaling {#Perform-Auto-Scaling-in-AutoCAD-to-PDF-in-CSharp}

The CAD drawing may consist of multiple layers where each layer might have a different dimension. In various scenarios, you may want to have a unified scaling in the converted PDF file. For such cases, you can configure the API to auto-scale the layers in accordance with the page size in the PDF document. The following are the steps to perform auto-scaling in AutoCAD to PDF conversion.

*   Load the DWG/DXF file using the [Image][27] class.
*   Create an instance of [CadRasterizationOptions][28] class.
*   Set [CadRasterizationOptions.AutomaticLayoutsScaling][29] to true.
*   Create an object of [PdfOptions][30] class and initialize [PdfOptions.VectorRasterizationOptions][31] property with _CadRasterizationOptions_ object.
*   Convert CAD drawing to PDF using [Image.Save(String, ImageOptionsBase)][32] method.

The following code sample shows how to convert CAD drawing to PDF with auto-scaling using C#.

{{< gist aspose-com-gists e20eb36e47c431f229254444d9722fd0 "autocad-to-pdf-auto-scaling.cs" >}}

## Modify Background and Drawing Color in Converted PDF {#Specify-Background-and-Drawing-Color-in-AutoCAD-to-PDF}

Aspose.CAD for .NET also lets you modify the default color scheme of the CAD drawings in the converted PDF document. The following are the steps to specify the background and drawing colors.

*   Load the DWG/DXF file using the [Image][33] class.
*   Create an instance of [CadRasterizationOptions][34] class.
*   Set background color using [CadRasterizationOptions.BackgroundColor][35] property.
*   Set drawing color using [CadRasterizationOptions.DrawColor][36] property.
*   Create an object of [PdfOptions][37] class and initialize [PdfOptions.VectorRasterizationOptions][38] property with _CadRasterizationOptions_ object.
*   Convert DWG/DXF to PDF using [Image.Save(String, ImageOptionsBase)][39] method.

The following code sample shows how to convert DWG/DXF drawing to PDF with customized background and drawing colors.

{{< gist aspose-com-gists e20eb36e47c431f229254444d9722fd0 "autocad-to-pdf-custom-colors.cs" >}}

## Convert Specific Layers of CAD to PDF using C# {#Convert-Specific-Layer-of-AutoCAD-Drawing-to-PDF}

In case there are multiple layers in the AutoCAD drawing, you can specify the layers you want to have in the converted PDF document. For this, you can provide the list of the layers' names to the API using [CadRasterizationOptions.Layers][40] property. The following code sample shows how to convert a specific layer of the AutoCAD drawing to PDF using C#.

{{< gist aspose-com-gists e20eb36e47c431f229254444d9722fd0 "autocad-to-pdf-layers.cs" >}}

## Conclusion

In this article, you have seen how to convert CAD's DWG or DXF files to PDF using C#. Furthermore, you have learned how to customize the CAD to PDF conversion in various scenarios using Aspose.CAD for .NET API. You can explore more about the API using the [documentation][41].

## See Also

*   [Add Text and Image to DWG Files using C#][42]




[1]: https://en.wikipedia.org/wiki/AutoCAD
[2]: https://docs.fileformat.com/cad/dwg/
[3]: https://docs.fileformat.com/cad/dxf/
[4]: https://products.aspose.app/cad/viewer
[5]: https://en.wikipedia.org/wiki/Computer-aided_design
[6]: https://docs.fileformat.com/cad/dwg/
[7]: https://docs.fileformat.com/cad/dxf/
[8]: https://products.aspose.app/cad/viewer
[9]: #CSharp-AutoCAD-to-PDF-Converter-API
[10]: #Convert-AutoCAD-Drawing-to-PDF-using-CSharp
[11]: #Set-Canvas-Size-in-AutoCAD-to-PDF-using-CSharp
[12]: #Perform-Auto-Scaling-in-AutoCAD-to-PDF-in-CSharp
[13]: #Specify-Background-and-Drawing-Color-in-AutoCAD-to-PDF
[14]: #Convert-Specific-Layer-of-AutoCAD-Drawing-to-PDF
[15]: https://products.aspose.com/cad/net
[16]: https://downloads.aspose.com/cad/net
[17]: https://apireference.aspose.com/cad/net/aspose.cad/image
[18]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pdfoptions
[19]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[20]: https://apireference.aspose.com/cad/net/aspose.cad/image
[21]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[22]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions/properties/pagewidth
[23]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions/properties/pageheight
[24]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pdfoptions
[25]: https://apireference.aspose.com/cad/net/aspose.cad/imageoptionsbase/properties/vectorrasterizationoptions
[26]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[27]: https://apireference.aspose.com/cad/net/aspose.cad/image
[28]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[29]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions/properties/automaticlayoutsscaling
[30]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pdfoptions
[31]: https://apireference.aspose.com/cad/net/aspose.cad/imageoptionsbase/properties/vectorrasterizationoptions
[32]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[33]: https://apireference.aspose.com/cad/net/aspose.cad/image
[34]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[35]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions/properties/backgroundcolor
[36]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions/properties/drawcolor
[37]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pdfoptions
[38]: https://apireference.aspose.com/cad/net/aspose.cad/imageoptionsbase/properties/vectorrasterizationoptions
[39]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[40]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions/properties/layers
[41]: https://docs.aspose.com/cad/net/getting-started/
[42]: https://blog.aspose.com/2018/03/14/support-for-adding-text-and-image-in-dwg-files/





