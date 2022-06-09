---
title: 'Convert Excel Files to Images using C++'
seoTitle: "Convert Excel Files to Images using C++ | Excel to PNG, JPEG, TIFF, GIF"
description: "Convert Microsoft Excel files to Images using C++. Convert Excel to PNG, JPEG, GIF, TIFF, SVG, and other image formats with C++."
date: Thu, 28 Jan 2021 09:26:16 +0000
draft: false
url: /2021/01/28/convert-excel-files-to-images-using-cpp/
author: Muhammad Ahmad
summary: 'There can be many reasons for converting Excel files to images like adding images to web pages, PDFs, Word Documents, PowerPoint Presentations, etc. In this article, we will learn **how to convert Excel files to images with C++**.'
tags: ['Convert Excel files to Image Format', 'Convert Excel to Image C++', 'Excel to Images', 'Excel to PNG', 'Excel to PNG C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-Image.jpg" alt="Excel to Image">}}


There can be many reasons for converting Excel files to images. For instance, you can add images to web pages, PDFs, Word Documents, PowerPoint Presentations, etc. In this article, you will learn **how to convert Excel files to images with C++**.

*   [C++ Excel to Image Converter API][1]
*   [Excel to Image Conversion with C++][2]
*   [Get a Free License][3]

## C++ Excel to Image Converter API {#CPP-Excel-to-Image-Converter-API}

[Aspose.Cells for C++][4] is a native C++ library that enables you to create, manipulate and convert spreadsheets without requiring Microsoft Excel or Office Automation. Furthermore, the API provides built-in support to convert Excel spreadsheets to different formats as well. You can install Aspose.Cells for C++ API by either using the [NuGet][5] package or [downloading][6] the API directly.

## Excel to Image Conversion with C++ {#Excel-to-Image-Conversion-with-CPP}

Aspose.Cells for C++ allows you to convert Excel spreadsheets into various popular image formats. The following are the supported output image formats:

*   [BMP][7]
*   [EMF][8]
*   [EXIF][9]
*   [GIF][10]
*   [JPEG][11]
*   [PNG][12]
*   [SVG][13]
*   [TIFF][14]
*   [WMF][15]

You can use the following steps to convert Excel files to images.

*   Firstly, load the Excel file with the [IWorkbook][16] class.
*   Create an instance of the [IImageOrPrintOptions][17] class.
*   Set the image type by passing the ImageFormat enumeration to [IImageOrPrintOptions->SetImageFormat()][18] method.
*   Set other options like horizontal and vertical resolution with the [IImageOrPrintOptions][19] class.
*   Create an instance of the [IWorksheet][20] class with the worksheet that you want to convert.
*   Make an object of the [ISheetRender][21] class by passing the [IWorksheet][22] and the [IImageOrPrintOptions][23] instances as parameters.
*   Get the number of pages in the worksheet with the [ISheetRender->GetPageCount()][24] method.
*   Finally, loop through the pages and save each page as an image with the [ISheetRender->ToImage()][25] method.

The following example code snippet shows how to convert Excel files to images using C++.

{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "LoadingSavingAndConverting-ConvertingWorksheetToImage_PNG.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][26].

## Conclusion

To conclude, you have learned how to convert Excel spreadsheets to images using C++. By using Aspose.Cells for C++ API, you can convert Excel files to various popular image formats including PNG, TIFF, SVG, GIF, JPEG, etc. To explore more about the API, use the API [documentation][27].

## See Also

*   [Convert Excel Files to PDF using C++][28]




[1]: #CPP-Excel-to-Image-Converter-API
[2]: #Excel-to-Image-Conversion-with-CPP
[3]: #Get-a-Free-License
[4]: https://products.aspose.com/cells/cpp
[5]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[6]: https://downloads.aspose.com/cells/cpp
[7]: https://docs.fileformat.com/image/bmp/
[8]: https://docs.fileformat.com/image/emf/
[9]: https://docs.fileformat.com/image/exif/
[10]: https://docs.fileformat.com/image/gif/
[11]: https://docs.fileformat.com/image/jpeg/
[12]: https://docs.fileformat.com/image/png/
[13]: https://docs.fileformat.com/page-description-language/svg/
[14]: https://docs.fileformat.com/image/tiff/
[15]: https://docs.fileformat.com/image/wmf/
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_image_or_print_options
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_image_or_print_options#a07895b627359bb2f6fbfa7cb620b4d60
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_image_or_print_options
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_sheet_render
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_image_or_print_options
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_sheet_render#a13f251d2a31714a530aca069e77886b3
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.rendering.i_sheet_render#a80d01c810678a541f294155064a75f46
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/cells/cpp/
[28]: https://blog.aspose.com/2021/01/19/Convert-Excel-to-PDF-using-Cpp/





