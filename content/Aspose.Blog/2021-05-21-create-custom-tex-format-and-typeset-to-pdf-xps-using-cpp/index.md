---
title: 'Create Custom TeX Format and Typeset to PDF, XPS using C++'
seoTitle: "Create Custom TeX Format and Typeset to PDF, XPS using C++"
description: "Create custom TeX format and typeset it to PDF or XPS format programmatically using C++. Convert custom TeX format to PDF or XPS format."
date: Fri, 21 May 2021 15:16:35 +0000
draft: false
url: /2021/05/21/create-custom-tex-format-and-typeset-to-pdf-xps-using-cpp/
author: Muhammad Ahmad
summary: '[TeX][1] is a typesetting system that has been noted as one of the most sophisticated digital typographical systems. TeX is used for typesetting documents and generating outputs like [PDF][2], [XPS][3], and different image formats. There might be situations where you need to design a bunch of documents uniformly. For that, creating a custom TeX format will prove to be helpful. To that end, this article will teach you **how to create a custom TeX format and typeset it to PDF and XPS format**.'
tags: ['Create Custom TeX Format C++', 'Typeset Custom TeX Format To PDF C++', 'Typeset Custom TeX Format To XPS C++']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeX-to-PDF-XPS-1.png" alt="Create Custom TeX Format and Typeset to PDF and XPS using C++">}}


[TeX][4] is a typesetting system that has been noted as one of the most sophisticated digital typographical systems. TeX is used for typesetting documents and generating outputs like [PDF][5], [XPS][6], and different image formats. There might be situations where you need to design a bunch of documents uniformly. For that, creating a custom TeX format will prove to be helpful. To that end, this article will teach you **how to create a custom TeX format and typeset it to PDF and XPS formats using C++**.

*   [C++ API for Creating Custom TeX Format and Typesetting it to PDF and XPS][7]
*   [Create a Custom TeX Format using C++][8]
*   [Typeset Custom TeX Format to XPS Format][9]
*   [Typeset Custom TeX Format to PDF Format][10]

## C++ API for Creating Custom TeX Format and Typesetting it to PDF and XPS {#CPP-API-for-Creating-Custom-TeX-Format-and-Typesetting-it-to-PDF-and-XPS}

[Aspose.TeX for C++][11] is a C++ library for working with TeX files without requiring any additional software to be installed. The API allows you to typeset TeX files, create custom TeX format, and generate output in formats like XPS, PDF, PNG, JPEG, TIFF, BMP. You can either install the API through [NuGet][12] or download it directly from the [Downloads][13] section.

```
PM> Install-Package Aspose.TeX.Cpp
```

## Create a Custom TeX Format using C++ {#Create-a-Custom-TeX-Format-using-CPP}

The following are the steps to create a custom TeX format.

*   Create an instance of the [TeXOptions][14] class using the [TeXConfig::get\_ObjectIniTeX()][15] property value.
*   Specify the input and output working directories.
*   Create the format using the [TeX::CreateFormat(System::String path, System::SharedPtr<TeXOptions> options)][16] method.

The following sample code demonstrates how to create a custom TeX format using C++.

{{< gist aspose-com-gists b317c0983a91c26774d737023745b018 "Create-Custom-TeX-Format.cpp" >}}

## Typeset Custom TeX Format to XPS Format {#Typeset-Custom-TeX-Format-to-XPS-Format}

The following are the steps for typesetting custom TeX format to XPS format.

*   Create an instance of the [IWorkingDirectory][17] class to represent the input working directory.
*   Load the TeX file using the [FormatProvider][18] class.
*   Create an instance of the [TeXOptions][19] class using the [FormatProvider][20] object created previously.
*   Set the [JobName][21], [InputWorkingDirectory][22], and [OutputWorkingDirectory][23].
*   Use the [Typeset(System::SharedPtr<System::IO::Stream> stream, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][24] method and pass [XpsDevice][25] object as an argument to create the XPS output.

The following is the sample code to typeset a custom TeX format to XPS format.

{{< gist aspose-com-gists b317c0983a91c26774d737023745b018 "Typeset-Custom-TeX-To-Xps.cpp" >}}

## Typeset Custom TeX Format to PDF Format {#Typeset-Custom-TeX-Format-to-PDF-Format}

The following are the steps for typesetting custom TeX format to PDF format.

*   Create an instance of the [IWorkingDirectory][26] class to represent the input working directory.
*   Load the TeX file using the [FormatProvider][27] class.
*   Create an instance of the [TeXOptions][28] class using the [FormatProvider][29] object created previously.
*   Set the [JobName][30], [InputWorkingDirectory][31], and [OutputWorkingDirectory][32].
*   Create an instance of the [PdfSaveOptions][33] class and pass it to [TeXOptions->set\_SaveOptions(System::SharedPtr<Aspose::TeX::Presentation::SaveOptions> value)][34] method.
*   Use the [Typeset(System::SharedPtr<System::IO::Stream> stream, System::SharedPtr<Presentation::Device> device, System::SharedPtr<TeXOptions> options)][35] method and pass [PdfDevice][36] object as an argument to create the PDF output.

The following sample code shows how to typeset a custom TeX format to PDF format.

{{< gist aspose-com-gists b317c0983a91c26774d737023745b018 "Typeset-Custom-TeX-To-Pdf.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][37].

## Conclusion

In this article, you have learned how to create a custom TeX format using C++. Furthermore, you have learned how to typeset a custom TeX format to PDF and XPS formats using Aspose.TeX for C++ API. You can explore the API in detail by visiting the [official documentation][38]. In case of any questions, please feel free to reach us on our [free support forum][39].

## See Also

*   [Add or Remove Header and Footer in Word Documents using C++][40]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/page-description-language/xps/
[4]: https://docs.fileformat.com/page-description-language/tex/
[5]: https://docs.fileformat.com/pdf/
[6]: https://docs.fileformat.com/page-description-language/xps/
[7]: #CPP-API-for-Creating-Custom-TeX-Format-and-Typesetting-it-to-PDF-and-XPS
[8]: #Create-a-Custom-TeX-Format-using-CPP
[9]: #Typeset-Custom-TeX-Format-to-XPS-Format
[10]: #Typeset-Custom-TeX-Format-to-PDF-Format
[11]: https://products.aspose.com/tex/cpp
[12]: https://www.nuget.org/packages/Aspose.TeX.Cpp
[13]: https://downloads.aspose.com/tex/cpp
[14]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[15]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_config#aefa7bbdf2ed28d6499f2dc5d5ad2ca3e
[16]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#a7f424a7c3287bfbb61a1349b263f9d0a
[17]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.i_o.i_working_directory
[18]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.resource_providers.format_provider
[19]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[20]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.resource_providers.format_provider
[21]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a19a8e0f0a4dc0c7afb2b20736cfe1c6b
[22]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a4a62d572e9891fcd7ed3b8a6c55c22df
[23]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#aba38a2f3bb046f39f862ae417f2855e5
[24]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#ac3446cf925e7274a33b5ad2b271bf067
[25]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.xps.xps_device
[26]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.i_o.i_working_directory
[27]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.resource_providers.format_provider
[28]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options
[29]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.resource_providers.format_provider
[30]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a19a8e0f0a4dc0c7afb2b20736cfe1c6b
[31]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a4a62d572e9891fcd7ed3b8a6c55c22df
[32]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#aba38a2f3bb046f39f862ae417f2855e5
[33]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_save_options
[34]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x_options#a179635edfecc5682fb13067e6760fd73
[35]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.te_x#ac3446cf925e7274a33b5ad2b271bf067
[36]: https://apireference.aspose.com/tex/cpp/class/aspose.te_x.presentation.pdf.pdf_device
[37]: https://purchase.aspose.com/temporary-license
[38]: https://docs.aspose.com/tex/cpp/
[39]: https://forum.aspose.com/c/tex/47
[40]: https://blog.aspose.com/2021/05/17/add-or-remove-header-and-footer-in-word-documents-using-cpp/





