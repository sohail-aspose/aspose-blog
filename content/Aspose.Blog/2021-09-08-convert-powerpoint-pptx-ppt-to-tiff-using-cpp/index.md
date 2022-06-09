---
title: 'Convert PowerPoint PPTX/PPT to TIFF using C++'
seoTitle: "Convert PowerPoint PPTX/PPT to TIFF using C++"
description: "Convert PowerPoint PPTX/PPT files to TIFF images using C++. Set custom image size and pixel format for the generated TIFF images."
date: Wed, 08 Sep 2021 16:10:18 +0000
draft: false
url: /2021/09/08/convert-powerpoint-pptx-ppt-to-tiff-using-cpp/
author: Muhammad Ahmad
summary: 'Tagged Image File Format ([TIFF][1] is an image format that is commonly used for print purposes due to its high quality. There might be cases where you need to convert your [PPTX][2]/[PPT][3] files to TIFF format for printing purposes. For that, this article will teach you **how to convert PowerPoint PPTX/PPT files to TIFF format programmatically using C++**.'
tags: ['Convert PowerPoint Files to TIFF Images C++', 'Convert PowerPoint Files to TIFF Images with Custom Image Size C++', 'Convert PowerPoint Files to TIFF Images with Custom Pixel Format C++', 'PPT to TIFF', 'PPTX to TIFF', 'PowerPoint to TIFF']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-TIFF.jpg" alt="PPT to TIFF using C++">}}


Tagged Image File Format ([TIFF][4] is an image format that is commonly used for print purposes due to its high quality. There might be cases where you need to convert your [PPTX][5]/[PPT][6] files to TIFF format for printing purposes. For that, this article will teach you **how to convert PowerPoint PPTX/PPT files to TIFF format programmatically using C++**.

*   [C++ API for Converting PowerPoint PPTX/PPT Files to TIFF Format][7]
*   [Convert PowerPoint Files to TIFF Format using C++][8]
*   [Converting PowerPoint Files to TIFF Format with Custom Image Size][9]
*   [Convert PowerPoint Files to TIFF Format with Custom Pixel Format][10]

**TIP:** You may want to check out **Aspose FREE online [PowerPoint to Poster Converter][11].**

## C++ API for Converting PowerPoint PPTX/PPT Files to TIFF Format {#CPP-API-for-Converting-PowerPoint-PPTX-PPT-Files-to-TIFF-Format}

[Aspose.Slides for C++][12] is a C++ API for working with PowerPoint files. It enables you to create, read and modify PPT and PPTX files without needing additional software. Furthermore, the API supports converting PPTX/PPT files to TIFF image format. You can either install the API through [NuGet][13] or download it directly from the [Downloads][14] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Convert PowerPoint Files to TIFF Format using C++ {#Convert-PowerPoint-Files-to-TIFF-Format-using-CPP}

You can convert your PowerPoint PPTX/PPT files to TIFF format in just a few lines of code. To achieve that, please follow the steps given below.

*   Load the PowerPoint file using the [Presentation][15] class.
*   Save the TIFF file using the [Presentation->Save (System::String name, Export::SaveFormat format)][16] method.

The following sample code shows how to convert PowerPoint files to TIFF format using C++.

{{< gist aspose-com-gists ec36fc0e95c6004860737b0a869e23f2 "Convert_PowerPoint_To_TIFF.cpp" >}}

## Converting PowerPoint Files to TIFF Format with Custom Image Size {#Converting-PowerPoint-Files-to-TIFF-Format-with-Custom-Image-Size}

The following are the steps to convert PowerPoint files to TIFF format with custom image size.

*   Load the PowerPoint file using the [Presentation][17] class.
*   Create an instance of the [TiffOptions][18] class.
*   Set the image size using the [TiffOptions->set\_ImageSize(System::Drawing::Size value)][19] method.
*   Save the TIFF file using the [Presentation->Save(System::String fname, Export::SaveFormat format, System::SharedPtr<Export::ISaveOptions> options)][20] method.

The following sample code shows how to convert PowerPoint files to TIFF images with custom image size using C++.

{{< gist aspose-com-gists ec36fc0e95c6004860737b0a869e23f2 "Convert_PowerPoint_To_TIFF_With_Custom_Image_Size.cpp" >}}

## Convert PowerPoint Files to TIFF Format with Custom Pixel Format {#Convert-PowerPoint-Files-to-TIFF-Format-with-Custom-Pixel-Format}

In order to set the pixel format, we will use the [ImagePixelFormat][21] enum. The [ImagePixelFormat][22] enum provides the following values.

*   **Format1bppIndexed**: 1 bit per pixel, indexed
*   **Format4bppIndexed**: 4 bits per pixel, indexed
*   **Format8bppIndexed**: 8 bits per pixel, indexed
*   **Format24bppRgb**: 24 bits per pixel, RGB
*   **Format32bppArgb**: 32 bits per pixel, ARGB

The following are the steps to convert a PPTX/PPT file to a TIFF image with custom pixel format using C++.

*   Load the PowerPoint file using the [Presentation][23] class.
*   Create an instance of the [TiffOptions][24] class.
*   Set the pixel format using the [TiffOptions->set\_PixelFormat(ImagePixelFormat value)][25] method.
*   Save the TIFF file using the [Presentation->Save(System::String fname, Export::SaveFormat format, System::SharedPtr<Export::ISaveOptions> options)][26] method.

The following sample code shows how to convert PowerPoint files to TIFF images with custom pixel format using C++.

{{< gist aspose-com-gists ec36fc0e95c6004860737b0a869e23f2 "Convert_PowerPoint_To_TIFF_With_Pixel_Format.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][27].

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX/PPT files to TIFF images using C++. Furthermore, you have learned how to set the custom image size and pixel format for the generated TIFF images. Aspose.Slides for C++ is a powerful API for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][28]. In case of any queries, please feel free to reach us at our [free support forum][29].

## See Also

*   [Convert PowerPoint to JPG using C++][30]
*   [Convert PowerPoint to PDF using C++][31]




[1]: https://docs.fileformat.com/image/tiff/)
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/image/tiff/)
[5]: https://docs.fileformat.com/presentation/pptx/
[6]: https://docs.fileformat.com/presentation/ppt/
[7]: #CPP-API-for-Converting-PowerPoint-PPTX-PPT-Files-to-TIFF-Format
[8]: #Convert-PowerPoint-Files-to-TIFF-Format-using-CPP
[9]: #Converting-PowerPoint-Files-to-TIFF-Format-with-Custom-Image-Size
[10]: #Convert-PowerPoint-Files-to-TIFF-Format-with-Custom-Pixel-Format
[11]: https://products.aspose.app/slides/conversion/convert-ppt-to-poster-online
[12]: https://products.aspose.com/slides/cpp
[13]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[14]: https://downloads.aspose.com/slides/cpp
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.tiff_options
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.tiff_options#ac270644c9de559a5d6cfb086e8b4da86
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a5c310c99c623922fc32e91a6d74f7020
[21]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.export#a5ab7a060e37eb300c64de4072559cb51
[22]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.export#a5ab7a060e37eb300c64de4072559cb51
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.tiff_options
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.tiff_options#a8f482df9f3320cc87d4261c02c1511c0
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a5c310c99c623922fc32e91a6d74f7020
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/slides/cpp/
[29]: https://forum.aspose.com/c/slides/11
[30]: https://blog.aspose.com/2021/03/06/convert-powerpoint-to-jpg-using-cpp/
[31]: https://blog.aspose.com/2021/03/03/convert-powerpoint-to-pdf-using-cpp/




