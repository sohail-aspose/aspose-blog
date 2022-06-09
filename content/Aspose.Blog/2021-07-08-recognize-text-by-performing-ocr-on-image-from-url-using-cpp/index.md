---
title: 'Recognize Text by Performing OCR on Image from URL using C++'
seoTitle: "Recognize Text by Performing OCR on Image from URL using C++"
description: "Recognize text by performing OCR on an online image using its URL with C++. Define recognition areas to perform OCR on only the selected image areas."
date: Thu, 08 Jul 2021 20:02:29 +0000
draft: false
url: /2021/07/08/recognize-text-by-performing-ocr-on-image-from-url-using-cpp/
author: Muhammad Ahmad
summary: 'Optical Character Recognition (OCR) is the process of extracting text from images. You may have online and offline images from which you might need to extract text information. You can perform OCR on offline images, but you might be thinking that to perform OCR on online images, you would have to download them. Well, that is not required. In this article, you will learn **how to perform OCR on images using their URL with C++**.'
tags: ['Perform OCR on an Image from URL C++', 'Recognize Text From Images C++', 'Recognize Text from Online Images C++', 'Recognize Text from Selected Image Areas C++']
categories: ['Aspose.OCR Product Family']
---

Optical Character Recognition (OCR) is the process of extracting text from images. You may have online and offline images from which you might need to extract text information. You can perform OCR on offline images, but you might be thinking that to perform OCR on online images, you would have to download them. Well, that is not required. In this article, you will learn **how to perform OCR on images using their URL with C++**.

*   [C++ API for Performing OCR on Images from URL][1]
*   [Recognize Text by Performing OCR on an Image from URL using C++][2]
*   [Recognize Text from Selected Image Areas by Defining Recognition Areas using C++][3]

## C++ API for Performing OCR on Images from URL {#CPP-API-for-Performing-OCR-on-Images-from-URL}

[Aspose.OCR for C++][4] is an optical character recognition API that can reliably perform OCR operations on images and scanned documents. The API also enables you to perform OCR on images from URLs. You can either install the API through [NuGet][5] or download it directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.OCR.Cpp
```

## Recognize Text by Performing OCR on an Image from URL using C++ {#Recognize-Text-by-Performing-OCR-on-an-Image-from-URL-using-CPP}

The following are the steps to perform OCR on images from URLs.

*   Prepare the buffer for the result.
*   Set the [RecognitionSettings][7].
*   Perform OCR on the image using the [asposeocr\_page\_from\_uri (const char \* uri, wchar\_t \* buffer, size\_t buffer\_size, RecognitionSettings settings)][8] method.

The following sample code shows how to perform OCR on an image from a URL using C++.

{{< gist aspose-com-gists 4c269d51138145682aec13d13f680a66 "Recongize_Image_From_Uri.cpp" >}}

## Recognize Text from Selected Image Areas by Defining Recognition Areas using C++ {#Recognize-Text-from-Selected-Image-Areas-by-Defining-Recognition-Areas-using-CPP}

If you do not want to perform OCR on the whole image and want to get the result from specific image areas, you can define recognition areas to do just that. The following are the steps to set recognition areas for the OCR operation.

*   Define the recognition areas in an array of [rect][9] structure.
*   Prepare the buffer for the result.
*   Set the value of the [RecognitionSettings.rectangles][10] struct member equal to the previously defined array of recognition areas.
*   Set the value of the [RecognitionSettings.rectangles\_size][11] struct member equal to the size of the recognition areas array.
*   Perform OCR on the image using the [asposeocr\_page\_from\_uri (const char \* uri, wchar\_t \* buffer, size\_t buffer\_size, RecognitionSettings settings)][12] method.

The following sample code demonstrates how to use recognition areas to recognize text from specific areas of an image using C++.

{{< gist aspose-com-gists 4c269d51138145682aec13d13f680a66 "Define_Recognition_Areas.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][13].

## Conclusion

In this article, you have learned how to perform OCR on images from any URL address using C++. Furthermore, you have seen how to define recognition areas to perform OCR on only selected areas of the image. Aspose.OCR for C++ is a robust API that provides many additional features for performing OCR on images. You can explore the API in detail by visiting the [official documentation][14]. In case of any questions, please feel free to reach us on our [free support forum][15].

## See Also

*   [Convert Image to Searchable PDF File with OCR using C++][16]
*   [Convert Image to Word Document (DOCX) with OCR using C++][17]




[1]: #CPP-API-for-Performing-OCR-on-Images-from-URL
[2]: #Recognize-Text-by-Performing-OCR-on-an-Image-from-URL-using-CPP
[3]: #Recognize-Text-from-Selected-Image-Areas-by-Defining-Recognition-Areas-using-CPP
[4]: https://products.aspose.com/ocr/cpp/
[5]: https://www.nuget.org/packages/Aspose.OCR.Cpp
[6]: https://downloads.aspose.com/ocr/cpp
[7]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings
[8]: https://apireference.aspose.com/ocr/cpp/groupAspose#gad893d81ccacd552e481334972e0b89f0
[9]: https://apireference.aspose.com/ocr/cpp/structrect
[10]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#a01c6acd22b406bce16f0df4f6d1be1ab
[11]: https://apireference.aspose.com/ocr/cpp/struct/recognition_settings#a960952c5c28ee2cb48505cda508fdb89
[12]: https://apireference.aspose.com/ocr/cpp/groupAspose#gad893d81ccacd552e481334972e0b89f0
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/ocr/cpp/
[15]: https://forum.aspose.com/c/ocr/16
[16]: https://blog.aspose.com/2021/06/14/convert-image-to-searchable-pdf-file-with-ocr-using-cpp/
[17]: https://blog.aspose.com/2021/06/16/convert-image-to-word-document-docx-with-ocr-using-cpp/





