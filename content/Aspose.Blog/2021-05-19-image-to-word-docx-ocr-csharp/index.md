---
title: 'Convert Image to Word Document (DOCX) with OCR using C#'
seoTitle: "Convert Image to Word Document DOCX by OCR using C# PNG JPG"
description: "You can convert image to word document DOCX programmatically using OCR C# in .NET. JPG PNG TIFF BMP Images to text with spell check using dictionaries."
date: Wed, 19 May 2021 12:17:00 +0000
draft: false
url: /2021/05/19/image-to-word-docx-ocr-csharp/
author: Farhan Raza
summary: 'You can convert an image containing text to an editable word document (DOCX) programmatically using C#. For instance, you need to convert an image captured from a scanner or a camera to an editable document then you need to perform OCR on the input image. You can go through further details under the following sections.'
tags: ['image to docx', 'image to word', 'image to word in Csharp', 'ocr to docx', 'ocr to word']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-DOCX-OCR-in-C.png" alt="Convert Image to Word DOCX OCR">}}


You can convert an image containing text to an editable word document ([DOCX][1] programmatically using C#. For instance, you need to convert an image captured from a scanner or a camera to an editable document then you need to perform OCR on the input image. You can go through further details under the following sections:

*   [Image to Word Document (DOCX) Converter in C# - Installation][2]
*   [Convert Image to Word Document with OCR Programmatically using C#][3]
*   [Convert Image to Word Document using Spell Checking with OCR in C#][4]

## Image to Word Document (DOCX) Converter in C# - Installation {#section1}

[Aspose.OCR for .NET][5] API can be used to recognize text from images. It supports converting images to text files or word documents (DOCX) as per your requirements. You can easily configure the API by downloading the DLL file from the [Downloads][6] section or via [NuGet Package Manager][7] with the following command:

```
PM> Install-Package Aspose.OCR
```

## Convert Image to Word Document with OCR Programmatically using C# {#section2}

Sometimes you get scanned or captured images of text that are not searchable or editable. In other words, you can convert an image to an editable and searchable word document (DOCX) with OCR programmatically. Moreover, you need to follow the steps below for performing an OCR on the image and saving the result as a DOCX word file:

1.  Firstly, initialize an instance of [AsposeOcr][8] class.
2.  Then recognize the input image.
3.  Finally, save the result in Microsoft Word Document format (DOCX).

The following code explains how to convert an image to Word document (DOCX) with OCR programmatically using C#:

{{< gist aspose-com-gists 3354720c8cd171a4934e0d7a9d0f6ce1 "OCR-Image-to-Word.cs" >}}

## Convert Image to Word Document using Spell Checking with OCR in C# {#section3}

You can recognize text in different languages and convert the image to a word document. The API supports multiple languages and lets you utilize the dictionaries to maximize the efficiency and authenticity of the output. Moreover, the following is a list of some popularly used dictionaries that are supported for spell checking against recognized text:

<figure class="wp-block-table is-style-stripes"><table><thead><tr><th>Name</th><th>Description</th></tr></thead><tbody><tr><td>Eng</td><td>English dictionary</td></tr><tr><td>Deu</td><td>German dictionary</td></tr><tr><td>Spa</td><td>Spanish dictionary</td></tr><tr><td>Fra</td><td>French dictionary</td></tr><tr><td>Swe</td><td>Swedish dictionary</td></tr></tbody></table></figure>

Moreover, you may refer to the [API References][9] to find the complete list of supported dictionaries so far.

Please follow the steps below for converting the image to a word document (DOCX) using spell checking with OCR:

1.  Firstly, instantiate an object of the [AsposeOcr][10] class.
2.  Recognize image with OCR using [RecognizeImage()][11] method.
3.  Finally, save the result in Word Document format with spellcheck.

The below code elaborates how to convert the text in an image to a word document (DOCX) programmatically using C# language:

{{< gist aspose-com-gists 3354720c8cd171a4934e0d7a9d0f6ce1 "OCR-Image-to-Word-Spellcheck.cs" >}}

## Get Free API License

Interested to test the API in its full capacity without evaluation limitations? You may request a [Free Temporary License][12].

## Conclusion

In conclusion, you have explored how to convert the text from an image to an editable or searchable word document with the OCR feature programmatically using C#. Moreover, you may take a look at the [API Documentation][13] to explore other features offered by the API. Furthermore, please feel free to contact us at the [Free Support Forum][14] for any of your queries.

## See Also

[Convert Image to Text using C# OCR Library][15]




[1]: https://docs.fileformat.com/word-processing/docx/)
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/ocr/net
[6]: https://downloads.aspose.com/ocr/net
[7]: https://www.nuget.org/packages/Aspose.OCR/
[8]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[9]: https://apireference.aspose.com/ocr/net/aspose.ocr.spellchecker/spellchecklanguage
[10]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[11]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeimage/index
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/ocr/net/
[14]: https://forum.aspose.com/c/ocr/16
[15]: https://blog.aspose.com/2020/05/28/perform-ocr-on-images-and-scanned-documents-using-csharp-vb.net/





