---
title: 'Convert PUB to Image using C++'
seoTitle: "Convert PUB to Image using C++ | PUB to JPG, PNG and TIFF"
description: "Convert Microsoft Publisher PUB files to JPG, PNG, and TIFF image formats using C++. Convert PUB files to images within your C++ applications."
date: Fri, 23 Jul 2021 22:43:55 +0000
draft: false
url: /2021/07/23/convert-pub-to-image-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft Publisher (PUB) files are used for printing or publishing information. There might be scenarios where you need to share these files, and the receiving party does not have access to Microsoft Publisher. In such cases, converting these files to images before sharing can prove to be helpful. To that end, this article will teach you **how to convert PUB files to various image formats using C++**.'
tags: ['Convert PUB to JPG using C++', 'Convert PUB to PNG using C++', 'Convert PUB to TIFF using C++']
categories: ['Aspose.PDF Product Family', 'Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-PNG-JPG-TIF-Image.jpg" alt="Convert PUB to Image using C++">}}


Microsoft Publisher (PUB) files are used for printing or publishing information. There might be scenarios where you need to share these files, and the receiving party does not have access to Microsoft Publisher. In such cases, converting these files to images before sharing can prove to be helpful. To that end, this article will teach you **how to convert PUB files to various image formats using C++**.

*   [C++ APIs for Converting PUB Files to Image Format][1]
*   [Convert PUB Files to JPG Images using C++][2]
*   [Convert PUB Files to PNG Images using C++][3]
*   [Converting PUB Files to TIFF Images using C++][4]

## C++ APIs for Converting PUB Files to Image Format {#CPP-APIs-for-Converting-PUB-Files-to-Image-Format}

We will use the [Aspose.PUB for C++][5] and [Aspose.PDF for C++][6] APIs to perform this conversion. The former is a library for working with Microsoft Publisher (PUB) files, whereas the latter is the library for creating, reading, and modifying PDF files. We will use the Aspose.PUB for C++ API to convert PUB files to PDF format and Aspose.PDF for C++ API to convert the generated PDF files to image format. You can either install the APIs through NuGet or download them directly from the [Downloads][7] section.

```
PM> Install-Package Aspose.PUB.Cpp
PM> Install-Package Aspose.PDF.Cpp
```

## Convert PUB Files to JPG Images using C++ {#Convert-PUB-Files-to-JPG-Images-using-CPP}

The following are the steps to convert PUB files to [JPG][8] images.

*   Load the PUB file using the [PubFactory::CreateParser(System::String fileName)][9] method.
*   Convert the PUB file to PDF format using the [ConvertToPdf(System::SharedPtr<Document> doc, System::String fileName)][10] method.
*   Load the generated PDF file using the [Document][11] class.
*   Loop through the pages of the PDF file.
*   Get the dimensions of the PDF page.
*   Create an instance of the [Resolution][12] class.
*   Instantiate the [JpegDevice][13] class by providing the width, height, and resolution.
*   Create an instance of the [FileStream][14] for the output image.
*   Convert the PDF page to JPG image using the [JpegDevice->Process(System::SharedPtr<Page> page, System::SharedPtr< System::IO::Stream > output)][15] method.
*   Close the stream.

The following sample code shows how to convert PUB files to JPG images using C++.

{{< gist aspose-com-gists 7a71627d380b9ab105d8a978a878bb0b "PUB_To_JPG.cpp" >}}

## Convert PUB Files to PNG Images using C++ {#Convert-PUB-Files-to-PNG-Images-using-CPP}

In order to convert PUB files to [PNG][16] images, follow the steps given below.

*   Load the PUB file using the [PubFactory::CreateParser(System::String fileName)][17] method.
*   Convert the PUB file to PDF format using the [ConvertToPdf(System::SharedPtr<Document> doc, System::String fileName)][18] method.
*   Load the generated PDF file using the [Document][19] class.
*   Loop through the pages of the PDF file.
*   Get the dimensions of the PDF page.
*   Create an instance of the [Resolution][20] class.
*   Instantiate the [PngDevice][21] class by providing the width, height, and resolution.
*   Create an instance of the [FileStream][22] for the output image.
*   Convert the PDF page to PNG image using the [PngDevice->Process(System::SharedPtr<Page> page, System::SharedPtr<System::IO::Stream> output)][23] method.
*   Close the stream.

The following sample code shows how to convert PUB files to PNG images using C++.

{{< gist aspose-com-gists 7a71627d380b9ab105d8a978a878bb0b "PUB_To_PNG.cpp" >}}

## Converting PUB Files to TIFF Images using C++ {#Converting-PUB-Files-to-TIFF-Images-using-CPP}

The following are the steps to convert PUB files to [TIFF][24] images.

*   Load the PUB file using the [PubFactory::CreateParser(System::String fileName)][25] method.
*   Convert the PUB file to PDF format using the [ConvertToPdf(System::SharedPtr<Document> doc, System::String fileName)][26] method.
*   Load the generated PDF file using the [Document][27] class.
*   Get the dimensions of the first PDF page.
*   Create an instance of the [Resolution][28] class.
*   Create an instance of the [TiffSettings][29] class and set the required settings.
*   Instantiate the [TiffDevice][30] class by providing the width, height, resolution, and [TiffSettings][31].
*   Create an instance of the [FileStream][32] for the output image.
*   Convert the PDF file to TIFF image using the [TiffDevice->Process( System::SharedPtr<Aspose::Pdf::Document> document, int32\_t fromPage, int32\_t toPage, System::SharedPtr<System::IO::Stream> output)][33] method.
*   Close the stream.

The following sample code demonstrates how to convert PUB files to TIFF images using C++.

{{< gist aspose-com-gists 7a71627d380b9ab105d8a978a878bb0b "PUB_To_TIFF.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][34].

## Conclusion

In this article, you have learned how to convert Microsoft Publisher (PUB) files to JPG, PNG, and TIFF images using C++. We used the Aspose.PUB for C++ and Aspose.PDF for C++ APIs to achieve this. You can explore these APIs in detail by visiting their official documentation. In case of any questions, please feel free to reach us at our [free support forum][35].

*   [Aspose.PUB for C++ Documentation][36]
*   [Aspose.PDF for C++ Documentation][37]

## See Also

*   [Extract Data from Tables in PDF Files using C++][38]




[1]: #CPP-APIs-for-Converting-PUB-Files-to-Image-Format
[2]: #Convert-PUB-Files-to-JPG-Images-using-CPP
[3]: #Convert-PUB-Files-to-PNG-Images-using-CPP
[4]: #Converting-PUB-Files-to-TIFF-Images-using-CPP
[5]: https://products.aspose.com/pub/cpp/
[6]: https://products.aspose.com/pdf/cpp
[7]: https://downloads.aspose.com/total
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.pub_factory#a88c04c4c35d45ee8febc7e1554d03c4b
[10]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.i_pdf_converter#acdea381bc8f2a2799e73a039b09ecdb5
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.resolution
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.jpeg_device
[14]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.jpeg_device#a2e855f4d9e418c524872f5266081d0e0
[16]: https://docs.fileformat.com/image/png/
[17]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.pub_factory#a88c04c4c35d45ee8febc7e1554d03c4b
[18]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.i_pdf_converter#acdea381bc8f2a2799e73a039b09ecdb5
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.resolution
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device
[22]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.png_device#ac84fc0ebb782c5d8522f0108d5826b0c
[24]: https://docs.fileformat.com/image/tiff/
[25]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.pub_factory#a88c04c4c35d45ee8febc7e1554d03c4b
[26]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.i_pdf_converter#acdea381bc8f2a2799e73a039b09ecdb5
[27]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[28]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.resolution
[29]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.tiff_settings
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.tiff_device
[31]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.tiff_settings
[32]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[33]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.devices.tiff_device#a0790daa96125c5638a645647e9678f0c
[34]: https://purchase.aspose.com/temporary-license
[35]: https://forum.aspose.com/
[36]: https://docs.aspose.com/pub/cpp/
[37]: https://docs.aspose.com/pdf/cpp/
[38]: https://blog.aspose.com/2021/07/14/extract-data-from-tables-in-pdf-files-using-cpp/





