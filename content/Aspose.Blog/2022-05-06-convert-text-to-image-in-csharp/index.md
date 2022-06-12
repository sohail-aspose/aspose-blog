---
title: 'Convert Text to PNG, JPEG, or GIF Image in C#'
seoTitle: "Convert Text to Image in C# .NET | TXT to PNG, JPEG, or GIF images"
description: "Use .NET word processing library to convert text to image in C#. Convert text in TXT files to PNG, JPEG, or GIF images in C# .NET."
date: Fri, 06 May 2022 10:48:00 +0000
draft: false
url: /2022/05/06/convert-text-to-image-in-csharp/
author: Usman Aziz
summary: 'In various cases, you have to convert the text into read-only formats such as images or PDFs. In a [previous article][1], we covered how to convert the text in a TXT file to PDF. For text to image conversion from within .NET applications, this article shows **how to convert a text to [PNG][2], [JPEG][3], or [GIF][4] image programmatically in C# .NET**.'
tags: ['Text to GIF in Csharp', 'Text to Image in Csharp', 'Text to JPG in Csharp', 'Text to png in Csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-Text-to-Image.png" alt="Convert Text to PNG, JPEG, and GIF Image in C#">}}


In various cases, you have to convert the text into read-only formats such as images or PDF. In a [previous article][5], we covered how to convert the text in a [TXT][6] file to PDF. For text to image conversion from within .NET applications, this article shows **how to convert a text to [PNG][7], [JPEG][8], or [GIF][9] image programmatically in C# .NET**.

*   [C# .NET API to Convert Text to Image][10]
*   [Convert Text (TXT) to Image in C#][11]

## Convert Text to PNG, JPEG, or GIF Images in C# - .NET API {#API-to-Convert-Text-to-Image}

To convert text to PNG, JPEG, or GIF images, we will use [Aspose.Words for .NET][12]. It is a powerful API that allows you to create and manipulate MS Word documents. Moreover, it lets you convert MS Word and text documents to various other file formats. You can [download][13] the API’s DLL or install it directly from [NuGet][14].

```
PM> Install-Package Aspose.Words
```

## Convert Text (TXT) to Image in C# {#Convert-Text-TXT-to-Image}

TXT files are the simplest and easiest way to store plain text without any formatting. Therefore, we will use a TXT file and convert its text into PNG, JPEG, or GIF images. The following are the steps to convert text to image in C#.

*   Load the text file using the [**Document**][15] class.
*   Loop through all the pages in the document.
*   Extract each page using [**Document.ExtractPages()**][16] method.
*   Save page as PNG (or another image format) using [**Document.Save()**][17] method.

The following code sample shows how to convert a text to images in C#.

\[gist id="f6b256d3266fc602d8e84e580b055488" file="convert-text-to-image.cs"\]

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][18] in order to use Aspose.Words for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert text to image programmatically in C#. You can use the provided code sample and convert the text in TXT files to PNG, JPEG, or GIF images seamlessly. Besides, you can explore other features offered by Aspose.Words for .NET using the [documentation][19]. Also, you can post your questions on our [forum][20].

## See Also

*   [Create MS Word Document in C#][21]
*   [Create Rich Word Documents in Java][22]


[1]: https://blog.aspose.com/2021/11/02/convert-txt-to-pdf-in-csharp/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/gif/
[5]: https://blog.aspose.com/2021/11/02/convert-txt-to-pdf-in-csharp/
[6]: https://docs.fileformat.com/word-processing/txt/
[7]: https://docs.fileformat.com/image/png/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/image/gif/
[10]: #API-to-Convert-Text-to-Image
[11]: #Convert-Text-TXT-to-Image
[12]: https://products.aspose.com/words/net/
[13]: https://downloads.aspose.com/words/net
[14]: https://www.nuget.org/packages/Aspose.Words
[15]: https://apireference.aspose.com/words/net/aspose.words/document/
[16]: https://reference.aspose.com/words/net/aspose.words/document/extractpages/
[17]: https://apireference.aspose.com/words/net/aspose.words/document/save
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/words/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[22]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/





