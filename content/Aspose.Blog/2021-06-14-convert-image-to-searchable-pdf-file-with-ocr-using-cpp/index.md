---
title: 'Convert Image to Searchable PDF File with OCR using C++'
seoTitle: "Convert Image to Searchable PDF File with OCR using C++"
description: "Convert Images to Searchable PDF files using C++. Convert JPEG, BMP, and PNG images to PDF format within your C++ applications."
date: Mon, 14 Jun 2021 19:13:20 +0000
draft: false
url: /2021/06/14/convert-image-to-searchable-pdf-file-with-ocr-using-cpp/
author: Muhammad Ahmad
summary: 'Images and scanned documents may contain textual information that you might need to process further. For this, performing OCR operations on such images may prove to be helpful. You can extract text from such images and save it as a searchable [PDF][1] file. To that end, this article will teach you **how to convert images to searchable PDF files using C++**.'
tags: ['Convert Image to Searchable PDF C++', 'Convert Skewed Image to Searchable PDF C++']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-PDF-OCR-in-C.png" alt="Image to PDF OCR C++">}}


Images and scanned documents may contain textual information that you might need to process further. For this, performing OCR operations on such images may prove to be helpful. You can extract text from such images and save it as a searchable [PDF][2] file. To that end, this article will teach you **how to convert images to searchable PDF files using C++**.

*   [C++ API for Converting Images to Searchable PDF Files][3]
*   [Convert Image to Searchable PDF File using C++][4]
*   [Convert Skewed Image to Searchable PDF File using C++][5]

## C++ API for Converting Images to Searchable PDF Files {#CPP-API-for-Converting-Images-to-Searchable-PDF-Files}

[Aspose.OCR for C++][6] is an optical character recognition API that can reliably perform OCR operations on images and scanned documents. The API also enables you to convert images to searchable PDFs. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.OCR.Cpp
```

## Convert Image to Searchable PDF File using C++ {#Convert-Image-to-Searchable-PDF-File-using-CPP}

Aspose.OCR for C++ provides you the ability to convert [JPEG][9], [BMP][10], and [PNG][11] images to searchable PDF files. To achieve this, please follow the steps given below:

*   Prepare the buffer for the result.
*   Set the value of [RecognitionSettings.save\_format][12] struct member as _file\_format::pdf_.
*   Perform the OCR operation on the image and save the PDF file using the [asposeocr\_page\_save(const char \* image\_path, const char \* save\_path, RecognitionSettings settings)][13] method.

The following sample code shows how to create a searchable PDF file from an image using C++:

{{< gist aspose-com-gists 782401e51497cec4542317a0b9e4e57f "Image-To-PDF.cpp" >}}



{{< figure align=center src="images/ImageToPdfOcrCpp-1024x679.png" alt="Screenshot of the source image and output PDF file" caption="Screenshot of the source image and output PDF file">}}


## Convert Skewed Image to Searchable PDF File using C++ {#Convert-Skewed-Image-to-Searchable-PDF-File-using-CPP}

The API also provides the ability to perform OCR operations on skewed images. The following are the steps to convert a skewed image to a searchable PDF file:

*   Prepare the buffer for the result.
*   Calculate the skew angle of the image using the [asposeocr\_get\_skew(const char \* image\_path)][14] method.
*   Set the value of [RecognitionSettings.save\_format][15] struct member as _file\_format::pdf_.
*   Specify the skew angle using [RecognitionSettings.skew][16] struct member.
*   Perform the OCR operation on the image and save the PDF file using the [asposeocr\_page\_save(const char \* image\_path, const char \* save\_path, RecognitionSettings settings)][17] method.

The following are the steps to convert a skewed image to a searchable PDF file using C++:

{{< gist aspose-com-gists 782401e51497cec4542317a0b9e4e57f "Skewed-Image-To-PDF.cpp" >}}



{{< figure align=center src="images/SkewedImageToPdfOcrCpp-1024x723.png" alt="Screenshot of the source image and output PDF file" caption="Screenshot of the source image and output PDF file">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][18].

## Conclusion

In this article, you have learned how to convert images to searchable PDF files using C++. With Aspose.OCR for C++ API, you can convert JPEG, BMP, and PNG images to PDF format. The API provides many additional features that you can explore in detail by visiting the [official documentation][19]. In case of any questions, please feel free to reach us on our [free support forum][20].

## See Also

*   [Insert or Delete Text/Image Watermarks in PDF Files using C++][21]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #CPP-API-for-Converting-Images-to-Searchable-PDF-Files
[4]: #Convert-Image-to-Searchable-PDF-File-using-CPP
[5]: #Convert-Skewed-Image-to-Searchable-PDF-File-using-CPP
[6]: https://products.aspose.com/ocr/cpp/
[7]: https://www.nuget.org/packages/Aspose.OCR.Cpp
[8]: https://downloads.aspose.com/ocr/cpp
[9]: https://docs.fileformat.com/image/jpeg/
[10]: https://docs.fileformat.com/image/bmp/
[11]: https://docs.fileformat.com/image/png/
[12]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#ac011403d84ee28fc62fe1d9bec824c2d
[13]: https://apireference.aspose.com/ocr/cpp/groupAspose#ga471631a25e3e645880b07975b4478d9d
[14]: https://apireference.aspose.com/ocr/cpp/groupAspose#gade7ffa77a033f6bc4417922cf5c8f1ee
[15]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#ac011403d84ee28fc62fe1d9bec824c2d
[16]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#accf812434a7002e70b10b0edc701a450
[17]: https://apireference.aspose.com/ocr/cpp/groupAspose#ga471631a25e3e645880b07975b4478d9d
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/ocr/cpp/
[20]: https://forum.aspose.com/c/ocr/16
[21]: https://blog.aspose.com/2021/06/02/insert-or-delete-text-image-watermarks-in-pdf-files-using-cpp/





