---
title: 'Rotate PDF Pages, Text or Images using C++'
seoTitle: "Rotate PDF Pages, Text or Images using C++ | Rotate Text and Images"
description: "Rotate pages, text, and images in PDF documents using C++. Rotate text and images with additional properties within your C++ applications."
date: Mon, 31 May 2021 18:07:18 +0000
draft: false
url: /2021/05/31/rotate-pdf-pages-text-or-image-using-cpp/
author: Muhammad Ahmad
summary: 'Let us explore the scenarios related to rotation in [PDF][1] documents. There might be situations where you might have an inverted scanned PDF document that you need to fix. You can fix such a document by rotating the pages of the document. You might also want to add text or image watermarks to a PDF document by rotating them. To that end, this article will teach you **how to rotate PDF pages, text, and images programmatically using C++**.'
tags: ['Rotate PDF Image C++', 'Rotate PDF Pages C++', 'Rotate PDF Text C++']
categories: ['Aspose.PDF Product Family']
---

Let us explore the scenarios related to rotation in [PDF][2] documents. There might be situations where you might have an inverted scanned PDF document that you need to fix. You can fix such a document by rotating the pages of the document. You might also want to add text or image watermarks to a PDF document by rotating them. To that end, this article will teach you **how to rotate PDF pages, text, and images programmatically using C++**.

*   [C++ API for Rotating PDF Pages, Text, and Images][3]
*   [Rotate PDF Pages using C++][4]
*   [Rotating Text on PDF Pages using C++][5]
*   [Rotate an Image on a PDF Page using C++][6]

## C++ API for Rotating PDF Pages, Text, and Images {#CPP-API-for-Rotating-PDF-Pages-Text-and-Images}

[Aspose.PDF for C++][7] is a C++ library that allows you to create, read and update PDF documents. In addition to this, the API supports rotating PDF pages, text, and images. You can either install the API through [NuGet][8] or download it directly from the [downloads][9] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Rotate PDF Pages using C++ {#Rotate-PDF-Pages-using-CPP}

Rotating pages with Aspose.PDF for C++ is a breeze. With just a few lines of code, you can rotate all the pages of the PDF document. The following are the steps to rotate PDF pages using C++.

*   Load the source PDF document using the [Document][10] class.
*   Loop through the pages of the document. In case you want to rotate only selected pages, you can define that logic within this loop.
*   Rotate each page using the [Page->set\_Rotate(Rotation value)][11] method.
*   Save the output PDF file using the [Document->Save(System::String outputFileName, SaveFormat format)][12] method.

The following sample code shows how to rotate PDF pages using C++.

{{< gist aspose-com-gists 9c56e3d998ac1ca9f176da93adcb24c1 "Rotate-All-Pages.cpp" >}}

## Rotating Text on PDF Pages using C++ {#Rotating-Text-on-PDF-Pages-using-CPP}

While adding text to PDF documents, you can change many text properties, including its angle. In the following example, we will add text to a PDF page and rotate it at an angle of 45 degrees. The following are the steps to achieve that.

*   Create an instance of the [Document][13] class to represent a new PDF document.
*   Add a new page to the PDF document.
*   Create an instance of the [TextFragment][14] class with the text you want to add.
*   Set the position, angle, and other properties of the text.
*   Add text to the PDF page using the [TextBuilder->AppendText(System::SharedPtr<TextFragment> textFragment)][15] method.
*   Save the output PDF file using the [Document->Save(System::String outputFileName, SaveFormat format)][16] method.

The following sample code demonstrates how to rotate text on a PDF page using C++.



## Rotate an Image on a PDF Page using C++ {#Rotate-an-Image-on-a-PDF-Page-using-CPP}

While adding images to PDF documents, you can set many properties like height, width, opacity, rotation, etc. In this example, we will add an image to a PDF page and rotate it at an angle of 90 degrees. The following are the steps to rotate an image on a PDF page.

*   Load the source PDF document using the [Document][17] class.
*   Create an instance of the [ImageStamp][18] class with the image you want to add.
*   Set rotation and other properties of the image.
*   Add the image to the PDF page using [Document->get\_Pages()->idx\_get(1)->AddStamp(System::SharedPtr<Stamp> stamp)][19] method.
*   Save the output PDF file using the [Document->Save(System::String outputFileName, SaveFormat format)][20] method.

The following sample code shows how to rotate an image on a PDF page using C++.



## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][21].

## Conclusion

In this article, you have learned how to rotate pages, text, and images in PDF documents using C++. Aspose.PDF for C++ is a vast API that provides many additional features for working with PDF files. You can explore the API in detail by visiting the [official documentation][22]. In case of any questions, please feel free to reach us on our [free support forum][23].

## See Also

*   [Working with Bookmarks in PDF Files using C++][24]
*   [Working with Annotations in PDF Files using C++][25]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #CPP-API-for-Rotating-PDF-Pages-Text-and-Images
[4]: #Rotate-PDF-Pages-using-CPP
[5]: #Rotating-Text-on-PDF-Pages-using-CPP
[6]: #Rotate-an-Image-on-a-PDF-Page-using-CPP
[7]: https://products.aspose.com/pdf/cpp
[8]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[9]: https://downloads.aspose.com/pdf/cpp
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page#a48d6fa64db1c67613d6cdb96573ececa
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a0184df207563187be7df37b8dbe443f6
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_builder#aee31f846c1fd834116ae61e2e0cef44d
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a0184df207563187be7df37b8dbe443f6
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.image_stamp
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page#a3b998038dedf5266b4d60586b1b53d02
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a0184df207563187be7df37b8dbe443f6
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/pdf/cpp/
[23]: https://forum.aspose.com/c/pdf/10
[24]: https://blog.aspose.com/2021/04/30/working-with-bookmarks-in-pdf-files-using-cpp/
[25]: https://blog.aspose.com/2021/04/14/working-with-annotations-in-pdf-files-using-cpp/





