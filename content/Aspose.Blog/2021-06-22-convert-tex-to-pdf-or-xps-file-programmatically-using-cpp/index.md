---
title: 'Convert TeX to PDF or XPS File Programmatically using C++'
seoTitle: "Convert TeX to PDF or XPS File Programmatically using C++"
description: "Convert TeX files to XPS and PDF format using C++. Convert zipped TeX files to zipped PDF files within your C++ applications."
date: Tue, 22 Jun 2021 18:19:19 +0000
draft: false
url: /2021/06/22/convert-tex-to-pdf-or-xps-file-programmatically-using-cpp/
author: Muhammad Ahmad
summary: '[TeX][1] files are used for typesetting different documents and books containing text, symbols, and arithmetic expressions. In addition, these files can generate outputs like [PDF][2], [XPS][3], and various image formats. In this article, you will learn **how to convert TeX files to XPS and PDF format using C++**.'
tags: ['Convert TeX ZIP directory to PDF ZIP Directory C++', 'Convert TeX to PDF Format C++', 'Convert TeX to XPS Format C++']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeX-to-PDF-XPS-1.png" alt="Convert TeX to PDF or XPS File Programmatically using C++">}}


[TeX][4] files are used for typesetting different documents and books containing text, symbols, and arithmetic expressions. In addition, these files can generate outputs like [PDF][5], [XPS][6], and various image formats. In this article, you will learn **how to convert TeX files to XPS and PDF format using C++**.

*   [C++ API for Converting TeX to PDF and XPS Format][7]
*   [Convert TeX to XPS Format using C++][8]
*   [Converting TeX to PDF Format using C++][9]
*   [Convert TeX ZIP directory to PDF ZIP Directory using C++][10]

## C++ API for Converting TeX to PDF and XPS Format {#CPP-API-for-Converting-TeX-to-PDF-and-XPS-Format}

[Aspose.TeX for C++][11] is a C++ library for working with TeX files without requiring any additional software to be installed. The API allows you to typeset TeX files and generate output in formats like [XPS][12], [PDF][13], [PNG][14], [JPEG][15], [TIFF][16], [BMP][17]. You can either install the API through [NuGet][18] or download it directly from the [Downloads][19] section.

```
PM> Install-Package Aspose.TeX.Cpp
```

## Convert TeX to XPS Format using C++ {#Convert-TeX-to-XPS-Format-using-CPP}

You can convert TeX files to XPS format in just a few lines of code. To achieve this, please follow the steps given below.

*   Create an instance of the [TeXOptions][20] class using the [TeXConfig::ObjectTeX(System::SharedPtr<Aspose::TeX::ResourceProviders::FormatProvider> formatProvider = nullptr)][21] member function.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Save the output XPS file using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][22] method with an instance of the [XpsDevice][23] class.

The following sample code demonstrates how to convert a TeX file to XPS format using C++.

{{< gist aspose-com-gists a520bd27ea4617951b3cc55b1dc2748e "Convert-TeX-to-XPS.cpp" >}}

## Converting TeX to PDF Format using C++ {#Converting-TeX-to-PDF-Format-using-CPP}

The following are the steps to convert TeX files to PDF format.

*   Create an instance of the [TeXOptions][24] class using the [TeXConfig::ObjectTeX(System::SharedPtr<Aspose::TeX::ResourceProviders::FormatProvider> formatProvider = nullptr)][25] member function.
*   Specify the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Pass an instance of the [PdfSaveOptions][26] class to the [TeXOptions->set\_SaveOptions(System::SharedPtr<Aspose::TeX::Presentation::SaveOptions> value)][27] method.
*   Save the output PDF file using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][28] method with an instance of the [PdfDevice][29] class.

The following sample code shows how to convert a TeX file to PDF format using C++.

{{< gist aspose-com-gists a520bd27ea4617951b3cc55b1dc2748e "Convert-TeX-to-PDF.cpp" >}}

## Convert TeX ZIP directory to PDF ZIP Directory using C++ {#Convert-TeX-ZIP-directory-to-PDF-ZIP-Directory-using-CPP}

In order to convert multiple TeX files to PDF format in one go, you can add the TeX files to a ZIP archive and convert them to zipped PDF files. The following are the steps to achieve this.

*   Load the input and output ZIP archives in streams.
*   Create an instance of the [TeXOptions][30] class using the [TeXConfig::ObjectTeX(System::SharedPtr<Aspose::TeX::ResourceProviders::FormatProvider> formatProvider = nullptr)][31] member function.
*   Set the input and output working directories.
*   Specify console or memory stream as an output terminal.
*   Pass an instance of the [PdfSaveOptions][32] class to the [TeXOptions->set\_SaveOptions(System::SharedPtr<Aspose::TeX::Presentation::SaveOptions> value)][33] method.
*   Save the zipped output PDF file using the [TeX::Typeset(System::String path, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][34] method with an instance of the [PdfDevice][35] class.

The following sample code shows how to convert TeX ZIP archive to PDF ZIP archive using C++.

{{< gist aspose-com-gists a520bd27ea4617951b3cc55b1dc2748e "Convert-Zip-TeX-to-Zip-PDF.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][36].

## Conclusion

In this article, you have learned how to convert TeX files to XPS and PDF format using C++. Furthermore, you have learned how to convert TeX files in a ZIP archive to zipped PDF files. Aspose.TeX for C++ provides many additional features for working with TeX files. You can explore the API in detail by visiting the [official documentation][37]. In case of any questions, please feel free to reach us on our [free support forum][38].

## See Also

*   [Create Custom TeX Format and Typeset to PDF, XPS using C++][39]
*   [Convert TeX Files to Images using C++][40]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/page-description-language/xps/
[4]: https://docs.fileformat.com/page-description-language/tex/
[5]: https://docs.fileformat.com/pdf/
[6]: https://docs.fileformat.com/page-description-language/xps/
[7]: #CPP-API-for-Converting-TeX-to-PDF-and-XPS-Format
[8]: #Convert-TeX-to-XPS-Format-using-CPP
[9]: #Converting-TeX-to-PDF-Format-using-CPP
[10]: #Convert-TeX-ZIP-directory-to-PDF-ZIP-Directory-using-CPP
[11]: https://products.aspose.com/tex/cpp
[12]: https://docs.fileformat.com/page-description-language/xps/
[13]: https://docs.fileformat.com/pdf/
[14]: https://docs.fileformat.com/image/png/
[15]: https://docs.fileformat.com/image/jpeg/
[16]: https://docs.fileformat.com/image/tiff/
[17]: https://docs.fileformat.com/image/bmp/
[18]: https://www.nuget.org/packages/Aspose.TeX.Cpp
[19]: https://downloads.aspose.com/tex/cpp
[20]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[21]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_config#a0e3d1feb32162aab9023665ea70972ee
[22]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[23]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.xps.xps_device
[24]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[25]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_config#a0e3d1feb32162aab9023665ea70972ee
[26]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_save_options
[27]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a179635edfecc5682fb13067e6760fd73
[28]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[29]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_device
[30]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[31]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_config#a0e3d1feb32162aab9023665ea70972ee
[32]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_save_options
[33]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a179635edfecc5682fb13067e6760fd73
[34]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a1e44671b868bbade85c8572fcbf6bb0b
[35]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_device
[36]: https://purchase.aspose.com/temporary-license
[37]: https://docs.aspose.com/tex/cpp/
[38]: https://forum.aspose.com/c/tex/47
[39]: https://blog.aspose.com/2021/05/21/create-custom-tex-format-and-typeset-to-pdf-xps-using-cpp/
[40]: https://blog.aspose.com/2021/08/06/convert-tex-files-to-images-using-cpp/





