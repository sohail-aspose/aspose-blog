---
title: 'Convert Excel XSLX or XLS to Images using C#'
seoTitle: "Convert Excel to Images in C# | XLSX or XLS to PNG, JPEG, BMP, TIFF"
description: "Convert MS Excel sheets to image format in C#. Convert Excel worksheets to PNG, JPEG, BMP, TIFF, EMF, WMF, TIFF, GIF, SVG, and other image formats in C#."
date: Fri, 01 Jan 2021 09:24:00 +0000
draft: false
url: /2021/01/01/convert-excel-files-to-images-in-csharp/
author: Usman Aziz
summary: 'In various scenarios, you may want to convert Excel spreadsheets to high-resolution images, for example, when you need to embed the spreadsheet content within your web or desktop applications. In this article, you will learn **how to convert Excel files to image formats using C#** from within the .NET applications.'
tags: ['Convert Excel to Image Csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-Image.jpg" alt="Excel to Image">}}


In various scenarios, you may want to convert Excel spreadsheets to high-resolution images, for example, when you need to embed the spreadsheet content within your web or desktop applications. In this article, you will learn **how to convert Excel XLSX or XLS to images using C#** from within the .NET applications.

*   [C# Excel to Image Converter API][1]
*   [Excel to Image C# Conversion][2]
*   [Get Free License][3]

## C# Excel to Image Converter API {#CSharp-Excel-to-Image-Converter-API}

[Aspose.Cells for .NET][4] is a C# class library that is designed to create and manipulate MS Excel spreadsheets. In addition to spreadsheet automation and manipulation features, the API also provides a built-in converter to convert Excel worksheets to image formats. You can either [download][5] the API's DLL or install it using [NuGet][6].

```
PM> Install-Package Aspose.Cells
```

## Excel XLSX to Image C# Conversion {#Excel-to-Image-CSharp-Conversion}

Aspose.Cells for .NET allows you to convert Excel worksheets into various popular image formats. The list includes:

*   [EMF][7]
*   [WMF][8]
*   [JPEG][9]
*   [PNG][10]
*   [BMP][11]
*   [GIF][12]
*   [TIFF][13]
*   [SVG][14]
*   [GLTF][15]
*   PICT
*   SVM
*   Office Compatible EMF

The following are the steps to convert an Excel worksheet to image using Aspose.Cells for .NET.

*   Load the Excel file using [Workbook][16] class.
*   Create an instance of [ImageOrPrintOptions][17] class.
*   Set image type using [ImageOrPrintOptions.ImageType][18] property.
*   Use [ImageType][19] enumeration to select the format of the output image such as JPEG, PNG, etc.
*   Select the worksheet you want to render in the [Worksheet][20] object.
*   Create an object of [SheetRender][21] and pass the [Worksheet][22] and [ImageOrPrintOptions][23] objects to its constructor.
*   Loop through the pages using [SheetRender.PageCount][24] property to save each page as image using [SheetRender.ToImage(Int32, String)][25] method.

The following code sample shows how to convert an Excel worksheet to an image using C#.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Articles-ConvertingWorksheetToImage-ConvertWorksheetToImageByPage-1.cs" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][26] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert MS Excel XLSX or XLS files to images using C#. Furthermore, you can convert the Excel files to JPEG, PNG, BMP, TIFF, EMF, and other popular image formats seamlessly. In order to explore more about the C# Excel API, visit the [documentation][27].

## See Also

*   [Create MS Excel Files in C# without MS Office][28]




[1]: #CSharp-Excel-to-Image-Converter-API
[2]: #Excel-to-Image-CSharp-Conversion
[3]: #Get-Free-License
[4]: https://products.aspose.com/cells/net
[5]: https://downloads.aspose.com/cells/net
[6]: https://www.nuget.org/packages/Aspose.Cells
[7]: https://docs.fileformat.com/image/emf/
[8]: https://docs.fileformat.com/image/wmf/
[9]: https://docs.fileformat.com/image/jpeg/
[10]: https://docs.fileformat.com/image/png/
[11]: https://docs.fileformat.com/image/bmp/
[12]: https://docs.fileformat.com/image/gif/
[13]: https://docs.fileformat.com/image/tiff/
[14]: https://docs.fileformat.com/page-description-language/svg/
[15]: https://docs.fileformat.com/3d/gltf/
[16]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[17]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/imageorprintoptions
[18]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/imageorprintoptions/properties/imagetype
[19]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/imagetype
[20]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[21]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/sheetrender
[22]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[23]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/imageorprintoptions
[24]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/sheetrender/properties/pagecount
[25]: https://apireference.aspose.com/cells/net/aspose.cells.rendering.sheetrender/toimage/methods/4
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/cells/net/getting-started/
[28]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





