---
title: 'Convert Image to Text using C++ OCR Library'
seoTitle: "Convert Image to Text using C++ OCR Library | PNG, JPG, BMP to Text"
description: "Use C++ OCR Library to convert image to text using C++. Perform OCR on JPEG, PNG, and BMP image and extract single or multi-line text."
date: Tue, 23 Jun 2020 02:34:59 +0000
draft: false
url: /2020/06/23/convert-image-to-text-using-cpp-ocr-library/
author: Usman Aziz
summary: ''
tags: ['Perform OCR on Image cpp', 'convert image to text cpp']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Perform-OCR-using-C.jpg" alt="Perform OCR using C++">}}


The [OCR][1] (Optical Character Recognition) technology lets you read and convert the text in the images or scanned documents to the machine-readable form. The OCR has various use cases that include reading codes from vouchers, making the text editable, self-service stores, converting printed documents into digital formats, and so on. Various OCR tools and libraries are available in the market, however, the reliability of the OCR results is a key factor. In this article, I'll show you how to create your own OCR application and **convert images to text programmatically using C++**.

*   [C++ OCR Library to Convert Image to Text][2]
*   [Convert Image Page to Text using C++][3]
*   [Perform OCR for an Image with Single Line using C++][4]
*   [Convert Particular Area of Image to Text in C++][5]

## C++ OCR Library to Convert Image to Text {#Convert-Image-to-Text-C++-OCR-Library}

Aspose offers a powerful [C++ OCR library][6] that uses deep learning to provide you more reliable and near to accurate OCR results. You can [download][7] the library files as well as a sample project from [GitHub][8].

## Convert Image Page to Text using C++ {#Convert-Image-Page-to-Text-using-C++}

Lets first check out the scenario in which the image contains a multi-line text. This could be the case when you have a scanned book where each page of the book contains a bunch of text lines. The following are the steps to convert image to text in this case.

*   Set the path of the image in a string variable.
*   Prepare a buffer to store the OCR results.
*   Perform OCR using aspose::ocr::page(const char \*image\_path, wchar\_t \*buffer, size\_t buffer\_size) function.
*   Print the results or save them in a file.

The following code sample shows how to perform OCR and convert image to text using C++.

{{< gist aspose-com-gists 41945dce2c829c0c2a99ccee0f7969c4 "convert-image-to-text.cpp" >}}

## Perform OCR for an Image with Single Line using C++ {#Perform-OCR-for-an-Image-with-Single-Line-using-C++}

In the previous example, we have converted an image having multiple text lines. However, there could be the case when the image contains only a single line of text such as the caption or a slogan. The following are the steps to perform OCR in such cases.

*   Use a string variable to set the path of the image.
*   Create a buffer to store the OCR results.
*   Perform OCR using aspose::ocr::line(const char \*image\_path, wchar\_t \*buffer, size\_t buffer\_size) function.
*   Save or print the OCR results.

The following code sample shows how to perform OCR on an image with a single line of text using C++.

{{< gist aspose-com-gists 41945dce2c829c0c2a99ccee0f7969c4 "convert-image-to-text-single-line.cpp" >}}

## Convert a Particular Area of Image to Text in C++ {#Convert-Particular-Area-of-Image-to-Text-in-C++}

You can also customize the API to limit the area of the image where you want to perform the OCR. In this case, you can create a rectangle on the image to access the desired area. The following are the steps to extract text from a particular area of the image.

*   Set the path of the image in a string variable.
*   Prepare a buffer to store the OCR results.
*   Perform OCR using aspose::ocr::page\_rect(const char \*image\_path, wchar\_t \*buffer, size\_t buffer\_size, int x, int y, int w, int h) function.
*   Print the OCR results.

The following code sample shows how to convert a particular area of the image to text using C++.

{{< gist aspose-com-gists 41945dce2c829c0c2a99ccee0f7969c4 "convert-image-to-text-area.cpp" >}}

## Conclusion

In this article, you have learned how to use Aspose' OCR library to **convert images to text in C++**. We have seen how to perform OCR on an image with single or multiple lines of text as well as read text from a particular area of an image. You can learn more about _Aspose.OCR for C++_ using the [documentation][9].

## See Also

*   [Perform OCR on Images using C#][10]




[1]: https://en.wikipedia.org/wiki/Optical_character_recognition
[2]: #Convert-Image-to-Text-C++-OCR-Library
[3]: #Convert-Image-Page-to-Text-using-C++
[4]: #Perform-OCR-for-an-Image-with-Single-Line-using-C++
[5]: #Convert-Particular-Area-of-Image-to-Text-in-C++
[6]: https://products.aspose.com/ocr/cpp
[7]: https://downloads.aspose.com/ocr/cpp
[8]: https://github.com/aspose-ocr/Aspose.OCR-for-C
[9]: https://docs.aspose.com/display/ocrcpp/Developer+Guide
[10]: https://blog.aspose.com/2020/05/28/perform-ocr-on-images-and-scanned-documents-using-csharp-vb.net/





