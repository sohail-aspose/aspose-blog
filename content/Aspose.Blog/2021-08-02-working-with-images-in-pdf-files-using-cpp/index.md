---
title: 'Working with Images in PDF Files using C++'
seoTitle: "Working with Images in PDF Files using C++ | Add, Extract, Delete Images"
description: "Manipulate images in PDF files using Aspose.PDF for C++ API. Add, extract, remove and replace images in PDF files using C++."
date: Mon, 02 Aug 2021 09:01:46 +0000
draft: false
url: /2021/08/02/working-with-images-in-pdf-files-using-cpp/
author: Muhammad Ahmad
summary: 'Images can be used to show a variety of things ranging from product photographs to workflows and flow charts. PDF files can contain images based on the type of information that it has. For example, a chair installation guide will include pictures of the chair demonstrating how to assemble it. There might be scenarios where you need to manipulate images in PDF files programmatically. For such cases, this article will teach you **how to work with images in PDF files using C++**.'
tags: ['Add Image to PDF using C++', 'Delete Image from PDF using C++', 'Extract Image from PDF using C++', 'Manipulate Images in PDF files using C++', 'Replace Image in PDF using C++']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Working with Images in PDF Files using C++">}}


Images can be used to show a variety of things ranging from product photographs to workflows and flow charts. PDF files can contain images based on the type of information that it has. For example, a chair installation guide will include pictures of the chair demonstrating how to assemble it. There might be scenarios where you need to manipulate images in PDF files programmatically. For such cases, this article will teach you **how to work with images in PDF files using C++**.

*   [C++ API for Working with Images in PDF Files][1]
*   [Add an Image to a PDF File using C++][2]
*   [Extract Images from a PDF File using C++][3]
*   [Remove an Image from a PDF File using C++][4]
*   [Replace an Image in a PDF File using C++][5]

## C++ API for Working with Images in PDF Files {#CPP-API-for-Working-with-Images-in-PDF-Files}

[Aspose.PDF for C++][6] is a robust C++ library that allows you to create, read, and modify PDF files. Furthermore, the API supports working with images in PDF documents. You can either install the API through [NuGet][7] or download it directly from the [downloads][8] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Add an Image to a PDF File using C++ {#Add-an-Image-to-a-PDF-File-using-CPP}

The following are the steps to add an image to a PDF file.

*   Load the PDF file using the [Document][9] class.
*   Retrieve the page where you want to add the image using the [Document->get\_Pages()->idx\_get(int32\_t index)][10] method.
*   Create an instance of the [Rectangle][11] class.
*   Add the image to the page using the [Page->AddImage(System::String imagePath, System::SharedPtr<Aspose::Pdf::Rectangle> rectangle)][12] method.
*   Save the PDF file using the [Document->Save(System::String outputFileName)][13] method.

The following sample code shows how to add an image to a PDF file using C++.

{{< gist aspose-com-gists fe6702a902f416508a722c2f08a6f499 "Add_Image_To_PDF.cpp" >}}

## Extract Images from a PDF File using C++ {#Extract-Images-from-a-PDF-File-using-CPP}

In order to extract images from a PDF file, follow the steps given below.

*   Load the PDF file using the [Document][14] class.
*   Extract the image using the [Document->get\_Pages()->idx\_get(int32\_t index)->get\_Resources()->get\_Images()->idx\_get(int32\_t index)][15] method.
*   Create an instance of the [FileStream][16] class to save the output image.
*   Save the image using the [XImage->Save(System::SharedPtr<System::IO::Stream> stream, System::SharedPtr<System::Drawing::Imaging::ImageFormat> format)][17] method.
*   Close the stream.

The following sample code demonstrates how to extract an image from a PDF file using C++.

{{< gist aspose-com-gists fe6702a902f416508a722c2f08a6f499 "Extract_Image_From_PDF.cpp" >}}

## Remove an Image from a PDF File using C++ {#Remove-an-Image-from-a-PDF-File-using-CPP}

The following are the steps to remove an image from a PDF file using C++.

*   Load the PDF file using the [Document][18] class.
*   Delete a particular image using the [Document->get\_Pages()->idx\_get(int32\_t index)->get\_Resources()->get\_Images()->Delete(int32\_t index)][19] method.
*   Save the PDF file using the [Document->Save(System::String outputFileName)][20] method.

The following sample code shows how to delete a particular image from a PDF file using C++.

{{< gist aspose-com-gists fe6702a902f416508a722c2f08a6f499 "Delete_Image_From_PDF.cpp" >}}

## Replace an Image in a PDF File using C++ {#Replace-an-Image-in-a-PDF-File-using-CPP}

In order to replace an existing image in a PDF file, follow the steps given below.

*   Load the PDF file using the [Document][21] class.
*   Open the new image using the [FileStream][22] class.
*   Replace the old image using the [Document->get\_Pages()->idx\_get(int32\_t index)->get\_Resources()->get\_Images()->Replace(int32\_t index, System::SharedPtr<System::IO::Stream> stream)][23] method.
*   Close the stream.
*   Save the PDF file using the [Document->Save(System::String outputFileName)][24] method.

The following code shows how to replace an image in a PDF file using C++.

{{< gist aspose-com-gists fe6702a902f416508a722c2f08a6f499 "Replace_Image_In_PDF.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][25].

## Conclusion

In this article, you have learned how to work with images in PDF files using C++. Specifically, you have learned how to add, extract, replace and remove images from PDF files using Aspose.PDF for C++ API. The API provides a bunch of additional features for working with PDF files that you can explore in detail by visiting the [official documentation][26]. In case of any queries, please feel free to reach us at our [free support forum][27].

## See Also

*   [Compress, or Optimize PDF Files with Same Quality using C++][28]




[1]: #CPP-API-for-Working-with-Images-in-PDF-Files
[2]: #Add-an-Image-to-a-PDF-File-using-CPP
[3]: #Extract-Images-from-a-PDF-File-using-CPP
[4]: #Remove-an-Image-from-a-PDF-File-using-CPP
[5]: #Replace-an-Image-in-a-PDF-File-using-CPP
[6]: https://products.aspose.com/pdf/cpp
[7]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[8]: https://downloads.aspose.com/pdf/cpp
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a30682a62c7630948c39bb950f47e4ba1
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.rectangle
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page#a9a10252b97d489ecfd994d487a6a3023
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.x_image_collection#a6697628ca2f5b954d2c9ba4a9475f319
[16]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.x_image#a8f5b3778db8cab911fa9ccfee809d2cd
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.x_image_collection#aa7b24de1441a5de8784eb174b0566cb2
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[22]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.x_image_collection#a698b65051b073f0f4b84b1235889bd72
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/pdf/cpp/
[27]: https://forum.aspose.com/c/pdf/10
[28]: https://blog.aspose.com/2021/07/06/compress-or-optimize-pdf-files-with-same-quality-using-cpp/





