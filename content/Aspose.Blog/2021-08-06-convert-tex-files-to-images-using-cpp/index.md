---
title: 'Convert TeX Files to Images using C++'
seoTitle: "Convert TeX Files to Images using C++ | TeX to JPG, PNG, TIFF, and BMP"
description: "Convert TeX files to image format using C++. Convert TeX to JPG, PNG, TIFF, and BMP image formats within your C++ applications."
date: Fri, 06 Aug 2021 11:51:23 +0000
draft: false
url: /2021/08/06/convert-tex-files-to-images-using-cpp/
author: Muhammad Ahmad
summary: '[TeX][1] is a typesetting system that has been noted as one of the most sophisticated digital typographical systems. TeX files are used for typesetting different documents and books containing text, symbols, and arithmetic expressions. Furthermore, these files can generate output in [PNG][2], [JPEG][3], [TIFF][4], and [BMP][5] image formats. In this article, you will learn **how to convert TeX files to images using C++**.'
tags: ['Convert TeX to BMP using C++', 'Convert TeX to Images using C++', 'Convert TeX to JPG using C++', 'Convert TeX to PNG using C++', 'Convert TeX to TIFF using C++']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeXToImageCpp1.jpg" alt="Convert TeX Files to Images using C++">}}


[TeX][6] is a typesetting system that has been noted as one of the most sophisticated digital typographical systems. TeX files are used for typesetting different documents and books containing text, symbols, and arithmetic expressions. Furthermore, these files can generate output in [PNG][7], [JPEG][8], [TIFF][9], and [BMP][10] image formats. In this article, you will learn **how to convert TeX files to images using C++**.

*   [C++ API for Converting TeX Files to Images][11]
*   [Convert TeX Files to JPG Images using C++][12]
*   [Converting TeX Files to PNG Images using C++][13]
*   [Convert TeX Files to TIFF Images using C++][14]
*   [Converting TeX Files to BMP Images using C++][15]

## C++ API for Converting TeX Files to Images {#CPP-API-for-Converting-TeX-Files-to-Images}

[Aspose.TeX for C++][16] is a C++ library for working with TeX files without installing any additional software. The API allows you to typeset TeX files and generate output in PNG, JPEG, TIFF, and BMP image formats. You can either install the API through [NuGet][17] or download it directly from the [Downloads][18] section.

```
PM> Install-Package Aspose.TeX.Cpp
```

## Convert TeX Files to JPG Images using C++ {#Convert-TeX-Files-to-JPG-Images-using-CPP}

The following are the steps to convert TeX files to JPG images.

*   Create an instance of the [TeXOptions][19] class using the [TeXOptions::ConsoleAppOptions(System::SharedPtr<TeXConfig> config)][20] method.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Set the save options to the instance of the [JpegSaveOptions][21] class.
*   Save the output JPG image using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][22] method with an instance of the [ImageDevice][23] class.

The following sample code shows how to convert a TeX file to a JPG image using C++.

{{< gist aspose-com-gists 36b5e72851c49250c8747cab3a94a381 "Convert_TeX_To_JPG.cpp" >}}

## Converting TeX Files to PNG Images using C++ {#Converting-TeX-Files-to-PNG-Images-using-CPP}

In order to convert TeX Files to PNG images, follow the steps given below.

*   Create an instance of the [TeXOptions][24] class using the [TeXOptions::ConsoleAppOptions(System::SharedPtr<TeXConfig> config)][25] method.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Set the save options to the instance of the [PngSaveOptions][26] class.
*   Save the output PNG image using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][27] method with an instance of the [ImageDevice][28] class.

The following sample code demonstrates how to convert a TeX file to a PNG image using C++.

{{< gist aspose-com-gists 36b5e72851c49250c8747cab3a94a381 "Convert_TeX_To_PNG.cpp" >}}

## Convert TeX Files to TIFF Images using C++ {#Convert-TeX-Files-to-TIFF-Images-using-CPP}

The following are the steps to convert TeX Files to TIFF images using C++.

*   Create an instance of the [TeXOptions][29] class using the [TeXOptions::ConsoleAppOptions(System::SharedPtr<TeXConfig> config)][30] method.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Set the save options to the instance of the [TiffSaveOptions][31] class.
*   Save the output TIFF image using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][32] method with an instance of the [ImageDevice][33] class.

The following sample code shows how to convert a TeX file to a TIFF image using C++.

{{< gist aspose-com-gists 36b5e72851c49250c8747cab3a94a381 "Convert_TeX_To_TIFF.cpp" >}}

## Converting TeX Files to BMP Images using C++ {#Converting-TeX-Files-to-BMP-Images-using-CPP}

The following are the steps to convert TeX files to BMP images using C++.

*   Create an instance of the [TeXOptions][34] class using the [TeXOptions::ConsoleAppOptions(System::SharedPtr<TeXConfig> config)][35] method.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Set the save options to the instance of the [BmpSaveOptions][36] class.
*   Save the output BMP image using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][37] method with an instance of the [ImageDevice][38] class.

The following sample code shows how to convert a TeX file to a BMP image using C++.

{{< gist aspose-com-gists 36b5e72851c49250c8747cab3a94a381 "Convert_TeX_To_BMP.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][39].

## Conclusion

In this article, you have learned how to convert TeX files to images using C++. Specifically, you have learned how to convert TeX files to JPG, PNG, TIFF, and BMP image formats using Aspose.TeX for C++ API. The API provides many additional features for working with TeX files. You can explore the API in detail by visiting the [official documentation][40]. In case of any queries, please feel free to reach us at our [free support forum][41].

## See Also

*   [Create Custom TeX Format and Typeset to PDF, XPS using C++][42]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/tiff/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/page-description-language/tex/
[7]: https://docs.fileformat.com/image/png/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/image/tiff/
[10]: https://docs.fileformat.com/image/bmp/
[11]: #CPP-API-for-Converting-TeX-Files-to-Images
[12]: #Convert-TeX-Files-to-JPG-Images-using-CPP
[13]: #Converting-TeX-Files-to-PNG-Images-using-CPP
[14]: #Convert-TeX-Files-to-TIFF-Images-using-CPP
[15]: #Converting-TeX-Files-to-BMP-Images-using-CPP
[16]: https://products.aspose.com/tex/cpp
[17]: https://www.nuget.org/packages/Aspose.TeX.Cpp
[18]: https://downloads.aspose.com/tex/cpp
[19]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[20]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#ad8aec9c3ff198c9b1e0f36927c44179d
[21]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.jpeg_save_options
[22]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[23]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.image_device
[24]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[25]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#ad8aec9c3ff198c9b1e0f36927c44179d
[26]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.png_save_options
[27]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[28]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.image_device
[29]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[30]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#ad8aec9c3ff198c9b1e0f36927c44179d
[31]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.tiff_save_options
[32]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[33]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.image_device
[34]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[35]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#ad8aec9c3ff198c9b1e0f36927c44179d
[36]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.bmp_save_options
[37]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[38]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.image.image_device
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/tex/cpp/
[41]: https://forum.aspose.com/c/tex/47
[42]: https://blog.aspose.com/2021/05/21/create-custom-tex-format-and-typeset-to-pdf-xps-using-cpp/





