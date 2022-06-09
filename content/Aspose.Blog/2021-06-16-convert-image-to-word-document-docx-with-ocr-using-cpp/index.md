---
title: 'Convert Image to Word Document (DOCX) with OCR using C++'
seoTitle: "Convert Image to Word Document (DOCX) with OCR using C++"
description: "Convert Images to Word Documents using C++. Convert JPEG, BMP, and PNG images to Word format within your C++ applications."
date: Wed, 16 Jun 2021 19:05:28 +0000
draft: false
url: /2021/06/16/convert-image-to-word-document-docx-with-ocr-using-cpp/
author: Muhammad Ahmad
summary: 'Images and scanned documents may contain textual information that you might need to process further. You might have captured pictures of text documents using your smartphone that you want to convert to editable documents. For this, performing OCR on the images can prove to be helpful. With OCR, you can convert images to searchable and editable Word documents. To that end, this article will teach you **how to convert images to Word documents using C++**.'
tags: ['Convert Image to Word Document C++', 'Convert Skewed Image to Word Document C++']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-DOCX-OCR-in-C.png" alt="Image to DOCX OCR C++">}}


Images and scanned documents may contain textual information that you might need to process further. You might have captured pictures of text documents using your smartphone that you want to convert to editable documents. For this, performing OCR on the images can prove to be helpful. With OCR, you can convert images to searchable and editable Word documents. To that end, this article will teach you **how to convert images to Word documents using C++**.

*   [C++ API for Converting Images to Word Documents][1]
*   [Convert Image to Word Document using C++][2]
*   [Convert Skewed Image to Word Document using C++][3]

## C++ API for Converting Images to Word Documents {#CPP-API-for-Converting-Images-to-Word-Documents}

[Aspose.OCR for C++][4] is an optical character recognition API that can extract text from images. The API also enables you to convert images to Word Documents like [DOC][5], [DOCX][6], and [TXT][7] files. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.OCR.Cpp
```

## Convert Image to Word Document using C++ {#Convert-Image-to-Word-Document-using-CPP}

Often you might need to search or edit the text in images, but you are unable to do so. By performing OCR on such images and converting them to Word documents, you can search and edit the text as needed. To achieve this, please follow the steps given below.

*   Prepare the buffer for the result.
*   Set the value of [RecognitionSettings.save\_format][10] struct member as _file\_format::docx_.
*   Perform the OCR operation on the image and save the Word file using the [asposeocr\_page\_save(const char \* image\_path, const char \* save\_path, RecognitionSettings settings)][11] method.

The following sample code shows how to convert an image to a Word document using C++:

{{< gist aspose-com-gists 95b3d43a8cf031d0bb0bd4f229741b4a "Image-To-Word-Document.cpp" >}}



{{< figure align=center src="images/ImageToWordOcrCpp-1024x676.png" alt="Screenshot of the source image and output Word file" caption="Screenshot of the source image and output Word file">}}


## Convert Skewed Image to Word Document using C++ {#Convert-Skewed-Image-to-Word-Document-using-CPP}

Images and scanned documents can sometimes be skewed. With Aspose.OCR for C++ API, you can perform OCR on skewed images. The following are the steps to convert a skewed image to a Word document:

*   Prepare the buffer for the result.
*   Calculate the skew angle of the image using the [asposeocr\_get\_skew(const char \* image\_path)][12] method.
*   Set the value of [RecognitionSettings.save\_format][13] struct member as _file\_format::docx_.
*   Specify the skew angle using [RecognitionSettings.skew][14] struct member.
*   Perform the OCR operation on the image and save the Word file using the [asposeocr\_page\_save(const char \* image\_path, const char \* save\_path, RecognitionSettings settings)][15] method.

The following sample code shows how to convert a skewed image to a Word document using C++:

{{< gist aspose-com-gists 95b3d43a8cf031d0bb0bd4f229741b4a "Skewed-Image-To-Word-Document.cpp" >}}



{{< figure align=center src="images/SkewedImageToWordOcrCpp-1024x679.png" alt="Screenshot of the source image and output Word file" caption="Screenshot of the source image and output Word file">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][16].

## Conclusion

In this article, you have learned how to convert images to Word documents using C++. Furthermore, you have seen how to calculate and use the skew angle of an image to perform OCR on skewed images. The API provides many additional features that you can explore in detail by visiting the [official documentation][17]. In case of any questions, please feel free to reach us on our [free support forum][18].

## See Also

*   [Convert Image to Text using C++ OCR Library][19]




[1]: #CPP-API-for-Converting-Images-to-Word-Documents
[2]: #Convert-Image-to-Word-Document-using-CPP
[3]: #Convert-Skewed-Image-to-Word-Document-using-CPP
[4]: https://products.aspose.com/ocr/cpp/
[5]: https://docs.fileformat.com/word-processing/doc/
[6]: https://docs.fileformat.com/word-processing/docx/
[7]: https://docs.fileformat.com/word-processing/txt/
[8]: https://www.nuget.org/packages/Aspose.OCR.Cpp
[9]: https://downloads.aspose.com/ocr/cpp
[10]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#ac011403d84ee28fc62fe1d9bec824c2d
[11]: https://apireference.aspose.com/ocr/cpp/groupAspose#ga471631a25e3e645880b07975b4478d9d
[12]: https://apireference.aspose.com/ocr/cpp/groupAspose#gade7ffa77a033f6bc4417922cf5c8f1ee
[13]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#ac011403d84ee28fc62fe1d9bec824c2d
[14]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#accf812434a7002e70b10b0edc701a450
[15]: https://apireference.aspose.com/ocr/cpp/groupAspose#ga471631a25e3e645880b07975b4478d9d
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/ocr/cpp/
[18]: https://forum.aspose.com/c/ocr/16
[19]: https://blog.aspose.com/2020/06/23/convert-image-to-text-using-cpp-ocr-library/





