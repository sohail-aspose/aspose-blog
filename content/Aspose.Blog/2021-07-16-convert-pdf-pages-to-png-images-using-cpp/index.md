---
title: 'Convert PDF Pages to PNG Images using C++'
seoTitle: "Convert PDF Pages to PNG Images using C++ | PDF to PNG"
description: "Learn how to convert PDF pages to PNG images using the simple and easy to use Aspose.PDF for C++ API within you C++ applications."
date: Fri, 16 Jul 2021 19:02:18 +0000
draft: false
url: /2021/07/16/convert-pdf-pages-to-png-images-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a popular format for sharing and printing documents due to its consistent layout. However, you might find yourself in situations where you want to generate a cover image of the PDF file or embed its pages on a web page. In such cases, converting the PDF file to image format will prove to be helpful. To that end, this article will teach you **how to convert PDF pages to **[**PNG**][2]** images using C++**.'
tags: ['Convert PDF Pages to PNG Images using C++', 'Convert PDF page to PNG image using C++', 'Convert PDF to PNG C++']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-to-PNG.jpg" alt="Convert PDF Pages to PNG Images using C++">}}


[PDF][3] is a popular format for sharing and printing documents due to its consistent layout. However, you might find yourself in situations where you want to generate a cover image of the PDF file or embed its pages on a web page. In such cases, converting the PDF file to image format will prove to be helpful. To that end, this article will teach you **how to convert PDF pages to **[**PNG**][4]** images using C++**.

*   [C++ API for Converting PDF Pages to PNG Images][5]
*   [Convert PDF Pages to PNG Images using C++][6]
*   [Convert a Single PDF Page to a PNG Image using C++][7]

## C++ API for Converting PDF Pages to PNG Images {#CPP-API-for-Converting-PDF-Pages-to-PNG-Images}

[Aspose.PDF for C++][8] is a C++ library that allows you to create, read and update PDF documents. Furthermore, the API supports converting PDF pages to PNG images. You can either install the API through [NuGet][9] or download it directly from the [downloads][10] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Convert PDF Pages to PNG Images using C++ {#Convert-PDF-Pages-to-PNG-Images-using-CPP}

The following are the steps to convert PDF pages to PNG images.

*   Load the PDF file using the [Document][11] class.
*   Iterate through the pages of the PDF file.
*   Within the loop, create an instance of the [FileStream][12] class for the output image.
*   Create an instance of the [Resolution][13] class.
*   Create an instance of the [PngDevice][14] class.
*   Using the [Process (System::SharedPtr<Page> page, System::SharedPtr<System::IO::Stream> output)][15] method of the [PngDevice][16] class, save the image of the PDF page.

The following sample code demonstrates how to save the pages of a PDF file as PNG images using C++.

{{< gist aspose-com-gists 27a116c958c8271756c87ef3df9c0705 "PDF_To_PNG.cpp" >}}

## Convert a Single PDF Page to a PNG Image using C++ {#Convert-a-Single-PDF-Page-to-a-PNG-Image-using-CPP}

The following are the steps to convert a single page of a PDF file to a PNG image.

*   Load the PDF file using the [Document][17] class.
*   Retrieve the page that you want to convert using the [Document->get\_Pages()->idx\_get(int32\_t index)][18] method.
*   Create an instance of the [FileStream][19] class for the output image.
*   Instantiate an object of the [Resolution][20] class.
*   Create an instance of the [PngDevice][21] class.
*   Using the [Process (System::SharedPtr<Page> page, System::SharedPtr<System::IO::Stream> output)][22] method of the [PngDevice][23] class, save the image of the PDF page.

The following sample code shows how to convert a single PDF page to a PNG image using C++.

{{< gist aspose-com-gists 27a116c958c8271756c87ef3df9c0705 "Single_PDF_Page_To_PNG.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][24].

## Conclusion

In this article, you have learned how to convert the pages of a PDF file to PNG images using C++. You can convert all the pages or selected pages of PDF files to PNG images. Aspose.PDF for C++ is a robust API with many additional features for automating your PDF-related workflows. You can explore the API in detail by visiting the [official documentation][25]. In case of any questions, please feel free to reach us at our [free support forum][26].

## See Also

*   [Insert or Delete Text/Image Watermarks in PDF Files using C++][27]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/image/png/
[5]: #CPP-API-for-Converting-PDF-Pages-to-PNG-Images
[6]: #Convert-PDF-Pages-to-PNG-Images-using-CPP
[7]: #Convert-a-Single-PDF-Page-to-a-PNG-Image-using-CPP
[8]: https://products.aspose.com/pdf/cpp
[9]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[10]: https://downloads.aspose.com/pdf/cpp
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[12]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.resolution
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device#ac84fc0ebb782c5d8522f0108d5826b0c
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a30682a62c7630948c39bb950f47e4ba1
[19]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.resolution
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device#ac84fc0ebb782c5d8522f0108d5826b0c
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/pdf/cpp/
[26]: https://forum.aspose.com/c/pdf/10
[27]: https://blog.aspose.com/2021/06/02/insert-or-delete-text-image-watermarks-in-pdf-files-using-cpp/





