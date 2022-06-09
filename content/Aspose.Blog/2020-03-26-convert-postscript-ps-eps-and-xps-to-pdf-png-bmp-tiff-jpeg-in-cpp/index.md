---
title: 'Convert PostScript PS/EPS and XPS to PDF and Raster Images in C++'
seoTitle: ""
description: ""
date: Thu, 26 Mar 2020 16:12:53 +0000
draft: false
url: /2020/03/26/convert-postscript-ps-eps-and-xps-to-pdf-png-bmp-tiff-jpeg-in-cpp/
author: Usman Aziz
summary: ''
tags: ['Convert EPS to Image', 'Convert EPS to PDF', 'Convert PS to Image', 'Convert PS to PDF', 'Convert XPS to Image', 'Convert XPS to PDF']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/PostScript-XPS-to-PDF-and-Image-C.png" alt="PostScript XPS to PDF and Image C++">}}


In my [previous][1] post, I have shown you how easy it is to create or edit PostScript (PS/EPS) and XPS documents programmatically using [Aspose.Page for C++][2]. In this article, I'll demonstrate **how to convert PS/EPS or XPS documents to PDF or raster image** formats including **PNG, JPEG, TIFF, and BMP using C++**. The rest of the article is composed of the following sections:

*   [Convert a PostScript PS/EPS to PDF in C++][3]
*   [Convert a PostScript PS/EPS to Image in C++][4]
*   [Convert XPS to PDF in C++][5]
*   [Convert XPS to image in C++][6]

Before we start, I assume that you have downloaded _Aspose.Page for C++_ and referenced it in your C++ project. However, if you haven't, you can get it installed from [NuGet][7] or download the complete package along with a plug and play console application from the [Downloads][8] section. 

## Convert a PostScript PS/EPS to PDF in C++ {#Convert-a-PostScript-PS-EPS-document-to-PDF-in-C++}

The following are the steps to convert a PostScript PS/EPS document to PDF:

*   Create a [FileStream][9] object for the output PDF file.
*   Load the input PostScript document in a [FileStream][10] object.
*   Create and initialize the [PsDocument][11] object with the input stream.
*   Create and initialize the [PdfDevice][12] object with the output stream.
*   Process the document and save it as a PDF file using the [PsDocument->Save][13] method.

The following code sample shows how to convert a PostScript PS document to PDF in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "convert-postscript-to-pdf.cpp" >}}

## Convert a PostScript PS/EPS to Image in C++ {#Convert-a-PostScript-PS-EPS-document-to-Image-in-C++}

The following are the steps to convert PS/EPS to an image format.

*   Create an object of [ImageFormat][14] to set the format of the output image, i.e. PNG.
*   Load the input PostScript document in a [FileStream][15] object.
*   Create and initialize the [PsDocument][16] object with the input stream.
*   Create an object of [ImageDevice][17].
*   Process the document and save it as an image using the [PsDocument->Save][18] method.

The following code sample shows how to convert PostScript PS/EPS to image in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "convert-postscript-to-image.cpp" >}}

## Convert an XPS to PDF in C++ {#Convert-XPS-to-PDF-in-C++}

The following are the steps to convert an XPS document to PDF:

*   Create [FileStream][19] objects for input XPS and output PDF files.
*   Load the XPS document stream into an [XpsDocument][20] object.
*   Create an object of the [PdfDevice][21] class and initialize it with the output stream.
*   Convert the XPS document to PDF using the [XpsDocument->Save][22] method.

The following code sample shows how to convert the XPS document to PDF in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "convert-xps-to-pdf.cpp" >}}

## Convert an XPS to Image in C++ {#Convert-XPS-to-image-in-C++}

The following are the steps to convert an XPS document to raster image formats:

*   Load the input XPS document into a [FileStream][23] object.
*   Create an object of [XpsDocument][24] and initialize it with the input stream object.
*   Set the save options by creating an object of the [PngSaveOptions][25] class.
*   Convert XPS to image using [XpsDocument->Save][26] method.

The following code sample shows how to convert XPS to PNG image in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "convert-xps-to-image.cpp" >}}

For converting the XPS document to BMP, TIFF, and JPEG, please visit the following article.

*   [Save XPS as BMP][27]
*   [Save XPS as TIFF][28]
*   [Save XPS as JPEG][29]

## Learn more about Aspose.Page for C++

In this article, you have seen how to convert PS, EPS and XPS document to PDF, PNG, JPEG, TIFF, and BMP using C++. You can learn more about _Aspose.Page for C++_ using the [documentation][30] and the [source code examples][31].

## See Also

*   [Create or Edit XPS Documents Programmatically in C++][32]




[1]: https://blog.aspose.com/2020/03/24/create-or-edit-postscript-and-xps-documents-in-cpp/
[2]: https://products.aspose.com/page/cpp
[3]: #Convert-a-PostScript-PS-EPS-document-to-PDF-in-C++
[4]: #Convert-a-PostScript-PS-EPS-document-to-Image-in-C++
[5]: #Convert-XPS-to-PDF-in-C++
[6]: #Convert-XPS-to-image-in-C++
[7]: https://www.nuget.org/packages/Aspose.Page.Cpp/
[8]: https://downloads.aspose.com/page/cpp
[9]: https://apireference.aspose.com/cpp/page/class/system.i_o.file_stream/
[10]: https://apireference.aspose.com/cpp/page/class/system.i_o.file_stream/
[11]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.ps_document/
[12]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.device.pdf_device/
[13]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.ps_document/#a4b9a2e2843541dccdca20e05677b7611
[14]: https://apireference.aspose.com/cpp/page/class/system.drawing.imaging.image_format/
[15]: https://apireference.aspose.com/cpp/page/class/system.i_o.file_stream/
[16]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.ps_document/
[17]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.device.image_device/
[18]: https://apireference.aspose.com/cpp/page/class/aspose.page.e_p_s.ps_document/#a4b9a2e2843541dccdca20e05677b7611
[19]: https://apireference.aspose.com/cpp/page/class/system.i_o.file_stream/
[20]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/
[21]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.presentation.pdf.pdf_device/
[22]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a19cc14bc6974182a3fec540beba8edda
[23]: https://apireference.aspose.com/cpp/page/class/system.i_o.file_stream/
[24]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/
[25]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.presentation.image.png_save_options/
[26]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a19cc14bc6974182a3fec540beba8edda
[27]: https://docs.aspose.com/
[28]: https://docs.aspose.com/
[29]: https://docs.aspose.com/
[30]: https://docs.aspose.com/display/pagecpp/Getting+Started
[31]: https://github.com/aspose-page/Aspose.Page-for-C
[32]: https://blog.aspose.com/2020/03/24/create-or-edit-postscript-and-xps-documents-in-cpp/





