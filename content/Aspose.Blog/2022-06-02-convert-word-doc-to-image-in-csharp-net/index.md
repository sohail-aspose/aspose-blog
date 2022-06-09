---
title: 'Convert Word DOC to PNG, JPEG, BMP, GIF, or TIFF in C#'
seoTitle: "C# Convert Word DOC to PNG, JPEG, BMP, GIF, or TIFF | .NET Word API"
description: "Use .NET Word processing API to convert Word DOC or DOCX to PNG, JPEG, BMP, GIF, or TIFF images programmatically. Customize Word to image in conversion."
date: Thu, 02 Jun 2022 16:26:53 +0000
draft: false
url: /2022/06/02/convert-word-doc-to-image-in-csharp-net/
author: Usman Aziz
summary: 'Often you need to embed the pages of an MS Word document into your application programmatically. One of the most commonly used methods for such cases is the conversion of Word documents to image formats. In this article, you will learn **how to convert Word [DOC][1] or **[DOCX][2]** files to [PNG][3], [JPEG][4], [BMP][5], [GIF][6], or [TIFF][7] images using C# .NET**. Furthermore, we will demonstrate how to control the Word to image conversion using different options.'
tags: ['Convert Word Doc to BMP Csharp', 'Convert Word Doc to GIF Csharp', 'Convert Word Doc to JPG Csharp', 'Convert Word Doc to PNG Csharp', 'Convert Word Doc to TIFF Csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Image.jpg" alt="Convert Word DOC to PNG, JPEG, or BMP in C#">}}


Often you need to embed the pages of an MS Word document into your application programmatically. One of the most commonly used methods for such cases is the conversion of Word documents to image formats. In this article, you will learn **how to convert Word [DOC][8] or **[DOCX][9]** files to [PNG][10], [JPEG][11], [BMP][12], [GIF][13], or [TIFF][14] images using C# .NET**. Furthermore, we will demonstrate how to control the Word to image conversion using different options.

*   [.NET API for Word to Image Conversion][15]
*   [Convert a Word Document to Image][16]
*   [Control Word to Image Conversion][17]

## C# .NET API for Word DOC to Image Conversion {#API-for-Word-to-Image-Conversion}

[Aspose.Words for .NET][18] is a powerful API that allows you to create MS Word documents from scratch. Moreover, it lets you manipulate the existing Word documents for encryption, conversion, text extraction, etc. We will use this API to convert Word documents to image formats. You can [download][19] the API’s DLL or install it directly from [NuGet][20].

```
PM> Install-Package Aspose.Words
```

## C# Convert a Word DOC to PNG, JPEG, BMP, GIF, or TIFF {#Convert-a-Word-Document-to-PNG-JPEG-or-BMP}

Aspose.Words for .NET makes it quite easier for you to convert a Word DOC/DOCX to desired image format. You can set the output image format as PNG, JPEG, BMP, GIF, or TIFF using [**SaveFormat**][21] enum. For demonstration, let's convert a Word DOCX to a PNG image in C#.

*   Load the Word document using the **[Document][22]**  class.
*   Specify the output image format using ****[ImageSaveOptions][23]**** class.
*   Loop through the pages in the document.
*   Convert each page in Word document to an image using **[Document.Save(string, ImageSaveOptions)][24]** method.

The following code sample shows how to convert a Word DOCX to PNG images in C#.

{{< gist aspose-com-gists 885c4fef954369b69233a7067f1ad7db "word-to-image.cs" >}}

## Control DOC/DOCX to Image Conversion in C# {#Control-Word-to-Image-Conversion}

You can also control the Word to image conversion using different options. For example, you can set horizontal resolution, vertical resolution, overall resolution, scale, pixel format, brightness, color mode, contrast, and paper color. The following are the steps to customize Word to image conversion in C#.

*   Load the Word document using the ****[Document][25]**** class.
*   Specify the output image format using **[ImageSaveOptions][26]** class.
*   Set desired options such as **[ImageBrightness][27]**, **[ImageContrast][28]**, etc.
*   Loop through the pages in the document.
*   Convert each page to image using **[Document.Save(string, ImageSaveOptions)][29]** method.

The following code sample shows how to control Word to JPEG image conversion using different options.

{{< gist aspose-com-gists 885c4fef954369b69233a7067f1ad7db "word-to-image-custom.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][30] in order to use Aspose.Words for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Word documents to PNG, JPEG, BMP, GIF, or TIFF images in C#. Moreover, you have seen how to control Word to image conversion using different options. Apart from that, you can explore other features offered by Aspose.Words for .NET using the [documentation][31]. Also, you can post your questions on our [forum][32].

## See Also

*   [Create MS Word Document in C#][33]
*   [Create Rich Word Documents in Java][34]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/image/gif/
[7]: https://docs.fileformat.com/image/tiff/
[8]: https://docs.fileformat.com/word-processing/doc/
[9]: https://docs.fileformat.com/word-processing/docx/
[10]: https://docs.fileformat.com/image/png/
[11]: https://docs.fileformat.com/image/jpeg/
[12]: https://docs.fileformat.com/image/bmp/
[13]: https://docs.fileformat.com/image/gif/
[14]: https://docs.fileformat.com/image/tiff/
[15]: #API-for-Word-to-Image-Conversion
[16]: #Convert-a-Word-Document-to-PNG-JPEG-or-BMP
[17]: #Control-Word-to-Image-Conversion
[18]: https://products.aspose.com/words/net/
[19]: https://downloads.aspose.com/words/net
[20]: https://www.nuget.org/packages/Aspose.Words
[21]: https://apireference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/saveformat/
[22]: https://apireference.aspose.com/words/net/aspose.words/document/
[23]: https://apireference.aspose.com/words/net/aspose.words.saving/imagesaveoptions
[24]: https://apireference.aspose.com/words/net/aspose.words/document/save
[25]: https://apireference.aspose.com/words/net/aspose.words/document/
[26]: https://apireference.aspose.com/words/net/aspose.words.saving/imagesaveoptions
[27]: https://apireference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/imagebrightness/
[28]: https://apireference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/imagecontrast/
[29]: https://apireference.aspose.com/words/net/aspose.words/document/save
[30]: https://purchase.aspose.com/temporary-license
[31]: https://docs.aspose.com/words/net/
[32]: https://forum.aspose.com/
[33]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[34]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/




