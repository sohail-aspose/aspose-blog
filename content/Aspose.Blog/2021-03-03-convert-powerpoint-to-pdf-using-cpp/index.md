---
title: 'Convert PowerPoint to PDF using C++'
seoTitle: "Convert PowerPoint to PDF using C++ | Convert PPTX to PDF C++"
description: "Convert PowerPoint presentations to PDF format using C++. Convert PPTX and PPT files to PDF format within your C++ applications."
date: Wed, 03 Mar 2021 09:27:33 +0000
draft: false
url: /2021/03/03/convert-powerpoint-to-pdf-using-cpp/
author: Muhammad Ahmad
summary: 'Many organizations use PowerPoint presentations for meetings or other group discussion scenarios. There might be situations where you need to share the same information with other people. In such cases, you may either choose [PPTX][1] or [PDF][2] format. If the file is to be used for presentations only, then the PPTX file format is acceptable. But if the file is to be shared for information purposes, then the PDF format is a better and user-friendly option. In this article, you will learn **how to convert PowerPoint slides to PDF format using C++**.'
tags: ['Convert PPT to PDF C++', 'Convert PPTX to PDF C++', 'Convert PowerPoint to PDF C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-PPTX-to-PDF-1.png" alt="PowerPoint to PDF C++">}}


Many organizations use PowerPoint presentations in meetings or other group discussion scenarios. There might be situations where you need to share the same information with other people. In such cases, you may either choose [PPTX][3] or [PDF][4] format. If the file is to be used for presentations only, then the PPTX file format is acceptable. But if the file is to be shared for information purposes, then the PDF format is a better and user-friendly option. In this article, you will learn **how to convert PowerPoint slides to PDF format using C++**.

*   [C++ API for PowerPoint to PDF conversion][5]
*   [PowerPoint to PDF conversion using C++][6]
*   [Convert PowerPoint to PDF with additional options][7]
*   [Get a Free License][8]

**TIP:** The PowerPoint to PDF conversion process powered by Aspose.Slides has been implemented in Aspose's [free online PowerPoint to PDF Converter.][9]

## C++ API for PowerPoint to PDF conversion {#CPP-API-for-PowerPoint-to-PDF-conversion}

[Aspose.Slides for C++][10] is a C++ library for creating and reading PowerPoint documents without using Microsoft PowerPoint. In addition, it also supports converting PowerPoint files to PDF format. You can either install the API through [NuGet][11] or download it directly from the [Downloads][12] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Convert PowerPoint to PDF using C++ {#Convert-PowerPoint-to-PDF-using-CPP}

The following are the steps to convert PowerPoint presentations to PDF format.

*   Load the PowerPoint file using the [Presentation][13] class.
*   Use the [Presentation->Save (System::String name, Export::SaveFormat format)][14] method to save the presentation as a PDF file.

The following is the sample code to convert PowerPoint presentations to PDF using C++.

{{< gist aspose-com-gists d1aaf38b93ed4beb8a5ce4b1a0e8cd76 "Convert-Slides-To-PDF.cpp" >}}

## Convert PowerPoint to PDF with additional options {#Convert-PowerPoint-to-PDF-with-additional-options}

Aspose.Slides for C++ provides the [PdfOptions][15] class to customize the conversion of PowerPoint presentations to PDF format. The following are some of the options provided by the [PdfOptions][16] class.

*   [**Password**][17]: Set the password to protect the PDF file.
*   [**AccessPermissions**][18]: Set the PDF permissions using the [PdfAccessPermissions][19] enum.
*   [**TextCompression**][20]: Set the text compression to be used using the [PdfTextCompression][21] enum.
*   [**ShowHiddenSlides**][22]: Specify whether to include hidden slides in the converted PDF file.
*   [**JpegQuality**][23]: Set the value to determine the quality of JPEG images in the PDF file.
*   [**Compliance**][24]: Set the compliance level of the generated PDF file using the [PdfCompliance][25] enum.
*   [**EmbedFullFonts**][26]: Set whether to include full fonts or only the used subset in the generated PDF file.

The following are the steps to convert PowerPoint presentations to PDF format with additional options.

*   Load the PowerPoint presentation file using the [Presentation][27] class.
*   Create an instance of the [PdfOptions][28] class.
*   Set the desired options such as [ShowHiddenSlides][29].
*   Save the PowerPoint as PDF using the [Presentation->Save (System::String name, Export::SaveFormat format, System::SharedPtr<Export::ISaveOptions> options)][30] method.

The following is the sample code to convert PowerPoint to PDF with additional options.

{{< gist aspose-com-gists d1aaf38b93ed4beb8a5ce4b1a0e8cd76 "Convert-Slides-To-PDF-With-Additional-Options.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][31].

## Conclusion

In this article, you have learned how to convert PowerPoint presentations to PDF format programmatically using C++. In addition, you have learned how to customize the conversion of PowerPoint to PDF files using Aspose.Slides for C++ API. The API provides many additional features that you can explore in detail by using the [official documentation][32]. If you have any questions, please feel free to contact us on the [forum][33].

## See Also

*   [Create PowerPoint Presentations using C++][34]
*   [Convert Presentation to Webpage HTML Programmatically using C++][35]




[1]: https://docs.fileformat.com/presentation/pptx/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: https://docs.fileformat.com/pdf/
[5]: #CPP-API-for-PowerPoint-to-PDF-conversion
[6]: #Convert-PowerPoint-to-PDF-using-CPP
[7]: #Convert-PowerPoint-to-PDF-with-additional-options
[8]: #Get-a-Free-License
[9]: https://products.aspose.app/slides/conversion/ppt-to-pdf
[10]: https://products.aspose.com/slides/cpp
[11]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[12]: https://downloads.aspose.com/slides/cpp
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#ab42606dbbf983fe00cc45a19565391a7
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#a77c8ac31e834a761e521dcb6229d33ce
[19]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.export#a8a80eed4177a9fe0cefe91999e4ec353
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#ac759a0d35e0c555f7073cebf197feb49
[21]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.export#aeca6b27c8c207f9b0fe317689b25568e
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#ad11e5a17110d70456df91cc1a5dade23
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#a6bbf3bd303430757aa85ac9e3d184861
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#aa9dfc92dd22455248ac171c24876cb8f
[25]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.export#a7bc072a408477939257fec3029aa45ec
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#a0d553863e4ade0a255f6cabdefac2775
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options
[29]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.export.pdf_options#ad11e5a17110d70456df91cc1a5dade23
[30]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a5c310c99c623922fc32e91a6d74f7020
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/slides/cpp/
[33]: https://forum.aspose.com/c/slides/11
[34]: https://blog.aspose.com/2020/12/29/create-powerpoint-presentations-using-cpp/
[35]: https://blog.aspose.com/2020/09/04/convert-presentation-to-webpage-html-using-cpp/





