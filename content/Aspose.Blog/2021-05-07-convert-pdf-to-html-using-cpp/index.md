---
title: 'Convert PDF to HTML using C++'
seoTitle: "Convert PDF to HTML using C++ | Customized PDF to HTML conversion"
description: "Convert PDF documents to HTML format using C++. Customize the generated HTML using the additional conversion options provided by the Apose.PDF for C++ API."
date: Fri, 07 May 2021 04:26:19 +0000
draft: false
url: /2021/05/07/convert-pdf-to-html-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a standard document format that is widely used for exchanging documents between individuals and different organizations. Even though it is popular, it may not always be the ideal choice for showing content. For example, on web pages, [HTML][2] is the better choice for a more satisfying user experience. If you want to display the PDF content on a website, then converting it to HTML may prove to be helpful. In light of this, this article will teach you **how to convert PDF documents to HTML format using C++**.'
tags: ['Convert PDF to HTML C++', 'Convert PDF to HTML using Additional Options']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PdfToHtmlCpp.png" alt="Convert PDF to HTML using C++">}}


[PDF][3] is a standard document format that is widely used for exchanging documents between individuals and different organizations. Even though it is popular, it may not always be the ideal choice for showing content. For example, on web pages, [HTML][4] is the better choice for a more satisfying user experience. If you want to display the PDF content on a website, then converting it to HTML may prove to be helpful. In light of this, this article will teach you **how to convert PDF documents to HTML format using [C++][5]**.

*   [C++ API for Converting PDF Documents to HTML Format][6]
*   [Convert PDF Documents to HTML Format using C++][7]
*   [Convert PDF Documents to HTML Format with Additional Options using C++][8]

## C++ API for Converting PDF Documents to HTML Format {#CPP-API-for-Converting-PDF-Documents-to-HTML-Format}

[Aspose.PDF for C++][9] is a C++ library that allows you to create, read and update PDF documents. Furthermore, the API supports converting PDF files to HTML format. You can either install the API through [NuGet][10] or download it directly from the [downloads][11] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Convert PDF Documents to HTML Format using C++ {#Convert-PDF-Documents-to-HTML-Format-using-CPP}

Converting a PDF document to HTML format is a breeze with the Aspose.PDF for C++ API. You can perform the conversion with just two lines of code. To convert a PDF document to HTML format, please follow the steps given below.

*   Load the PDF document using the [Document][12] class.
*   Save the HTML output using the [Document->Save(System::String outputFileName, SaveFormat format)][13] method.

The following sample code shows how to convert PDF documents to HTML format using C++.

{{< gist aspose-com-gists a38f7642215d4281c357d6e1287dc816 "Convert-PDF-To-HTML.cpp" >}}

### Source PDF File



{{< figure align=center src="images/ConvertPdfToHtmlSourceCpp.png" alt="Source PDF file used in the sample code.">}}


### Output HTML File



{{< figure align=center src="images/ConvertPdfToHtmlOutputCpp.png" alt="Output HTML file generated by the sample code">}}


## Convert PDF Documents to HTML Format with Additional Options using C++ {#Convert-PDF-Documents-to-HTML-Format-with-Additional-Options-using-CPP}

The Aspose.PDF for C++ API provides you the ability to customize the HTML generated by the conversion process. For this, the API offers the [HtmlSaveOptions][14] class. The following are some of the options provided by the [HtmlSaveOptions][15] class.

*   **[FontSavingMode][16]**: It is used to set the font saving mode used during the conversion. The [FontSavingModes][17] enum is used to set its value.
*   **[RasterImagesSavingMode][18]**: It is used to set how the raster images should be handled during the conversion. The [RasterImagesSavingModes][19] enum is used to set its value.
*   **[LettersPositioningMethod][20]**: It sets the positioning of letters in words. The [LettersPositioningMethods][21] enum is used to set its value.
*   **[SpecialFolderForAllImages][22]**: It is used to set the path where the images will be saved.
*   **[SplitIntoPages][23]**: It sets whether each page of the PDF should be converted as a separate HTML page or the whole document should be converted to a single HTML file.
*   **[SplitCssIntoPages][24]**: When [SplitIntoPages][25] is set to **true**, [SplitCssIntoPages][26] sets whether the CSS should be saved as a single file or as a separate file for each HTML page.

The following are the steps to convert a PDF document to HTML format with additional options.

*   Load the PDF document using the [Document][27] class.
*   Create an instance of the [HtmlSaveOptions][28] class.
*   Set the desired options.
*   Save the HTML output using the [Document->Save(System::String outputFileName, System::SharedPtr<SaveOptions> options)][29] method.

The following is the C++ sample code that demonstrates the use of the [HtmlSaveOptions][30] class to customize the HTML output.

{{< gist aspose-com-gists a38f7642215d4281c357d6e1287dc816 "Convert-PDF-To-HTML-With-Additional-Options.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][31].

## Conclusion

In this article, you have learned how to convert PDF documents to HTML format using C++. Furthermore, you have learned how to use the additional options provided by the Aspose.PDF for C++ API to customize the generated HTML. The API provides many additional features for automating your PDF-related tasks. You can explore the API in detail by using the [official documentation][32]. If you have any questions, please feel free to reach us on the [free support forum][33].

## See Also

*   [Convert PDF to SVG Format using C++][34]
*   [Working with Annotations in PDF Files using C++][35]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/web/html/
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/web/html/
[5]: https://docs.fileformat.com/programming/cpp/
[6]: #CPP-API-for-Converting-PDF-Documents-to-HTML-Format
[7]: #Convert-PDF-Documents-to-HTML-Format-using-CPP
[8]: #Convert-PDF-Documents-to-HTML-Format-with-Additional-Options-using-CPP
[9]: https://products.aspose.com/pdf/cpp
[10]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[11]: https://downloads.aspose.com/pdf/cpp
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a0184df207563187be7df37b8dbe443f6
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#aa64fca3c2c5617c1b0b7740084b619d8
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#adeb2e6a5eb725a97b47f721714727ca2
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#acaf96a92a35b74c5257f44e88aa3412d
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#a2457e92f0b44f360631815a575db11d0
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#ac7f4aa57ab7e7e5e6c3389586fc70005
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#aaeac1bc8a372918a2990589771dd3eb0
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#a668bb8a7174815f737fe7c77e958a44e
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#a7fcf1703f9f6c62ea46ccfdbf80a6e47
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#aa5572c2f10cca2ba4302f12dc75b0117
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#a7fcf1703f9f6c62ea46ccfdbf80a6e47
[26]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options#aa5572c2f10cca2ba4302f12dc75b0117
[27]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[28]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options
[29]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.html_save_options
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/pdf/cpp/developer-guide/
[33]: https://forum.aspose.com/c/pdf/10
[34]: https://blog.aspose.com/2021/02/01/convert-pdf-to-svg-format-using-cpp/
[35]: https://blog.aspose.com/2021/04/14/working-with-annotations-in-pdf-files-using-cpp/




