---
title: 'Convert Image to Text using C# OCR Library'
seoTitle: "Convert Image to Text using C# OCR Library | PNG, JPG, BMP to Text"
description: "Perform OCR and convert images to text using C# or VB.NET. Convert PNG, JPG, BMP images to text using C# OCR Library within ASP.NET or any .NET application."
date: Thu, 28 May 2020 16:27:36 +0000
draft: false
url: /2020/05/28/perform-ocr-on-images-and-scanned-documents-using-csharp-vb.net/
author: Usman Aziz
summary: ''
tags: ['Convert images to text using Csharp', 'OCR on image using CSharp', 'Optical Character Recognition using Csharp', 'Perform OCR using CSharp']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Perform-OCR-using-C.jpg" alt="Perform OCR using C#">}}


The OCR (Optical Character Recognition) is a well known and widely used technology to recognize and read text from images and scanned documents. In the OCR operation, the characters on the images are scanned, recognized, and converted into the digital form. The converted text can be validated and saved to perform further operations. In this article, I'll show you **how to perform OCR to convert images to text** programmatically using C# within your .NET applications. The rest of the article is divided into the following sections.

*   [C# OCR Library - Installation][1]
*   [Convert Image to Text using C# OCR API][2]
*   [Perform OCR on Images having Single Line of Text][3]

## C# OCR Library - Installation {#CSharp-OCR-Library-Installation}

[Aspose.OCR for .NET][4] is a powerful OCR library that lets you scan and convert images to text quite easily. It doesn't require lengthy codes to get the OCR features up and running within your .NET applications. The following are the installation methods of the C# OCR Library.

### Install via NuGet Package Manager

Simply search for Aspose.OCR in NuGet Package Manager and install it.



{{< figure align=center src="images/C-OCR-Library.jpg" alt="C# OCR Library">}}


### Install via Package Manager Console

The following is the command to install Aspose.OCR via Package Manager Console.

```
PM> Install-Package Aspose.OCR
```

## Convert Image to Text using C# OCR API {#Perform-OCR-on-Images-using-CSharp}

Let's see how to perform OCR on an image that could possibly be a page of a scanned document. The following are the steps to perform this operation.

*   Create an instance of the [AsposeOcr][5] class.
*   Call [AsposeOcr.RecognizeImage(string)][6] method by passing the image's path and get the result into a string object.

The following code sample shows how to convert an image to text using C#.

{{< gist aspose-com-gists dad6b4a35169ed7893fd376e819d7626 "Examples-CSharp-PerformingandManagingOCR-PerformOCROnImage-1.cs" >}}

## Perform OCR on Image with a Single Line of Text {#Perform-OCR-on-Image-of-Line-using-CSharp}

In the previous example, we have performed OCR on the image which contained multiple lines of text. However, it is possible that the image contains only a single line of text. In such cases, you can tell the API to recognize the line only. The following are the steps to perform convert an image containing a single line text.

*   Create an object of the [AsposeOcr][7] class.
*   Call [AsposeOcr.RecognizeLine(string)][8] method and pass to it the path of the image file.
*   Get the result into a string object.

The following code sample shows how to perform OCR and convert an image containing a single line of text using C#.

{{< gist aspose-com-gists dad6b4a35169ed7893fd376e819d7626 "Examples-CSharp-PerformingandManagingOCR-RecognizeLine-1.cs" >}}

## Perform OCR for Non-English Characters

Aspose.OCR doesn't limit the OCR features for the English language and you can recognize the characters of other languages as well. The recognition process and the code will remain the same regardless of the text's language. The following is the set of characters that can be recognized by the Aspose's OCR API.

<figure class="wp-block-table aligncenter is-style-stripes"><table><tbody><tr><td>space</td><td>!</td><td>"</td><td>#</td><td>$</td><td>%</td><td>&amp;</td><td>'</td><td>(</td><td class="has-text-align-left" data-align="left">)</td></tr><tr><td>*</td><td>+</td><td>,</td><td>-</td><td>.</td><td>/</td><td>0</td><td>1</td><td>2</td><td class="has-text-align-left" data-align="left">3 </td></tr><tr><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td><td>:</td><td>;</td><td><</td><th class="has-text-align-left" data-align="left">=</th></tr><tr><td>></td><td>?</td><td>@</td><td>[</td><td>\</td><td>]</td><td>_</td><td>`</td><td>{</td><td class="has-text-align-left" data-align="left">| </td></tr><tr><td>}</td><td>~</td><td>A</td><td>B</td><td>C</td><td>D</td><td>E</td><td>F</td><td>G</td><td class="has-text-align-left" data-align="left">H </td></tr><tr><td>I</td><td>J</td><td>K</td><td>L</td><td>M</td><td>N</td><td>O</td><td>P</td><td>Q</td><td class="has-text-align-left" data-align="left">R</td></tr><tr><td>S</td><td>T</td><td>U</td><td>V</td><td>W</td><td>X</td><td>Y</td><td>Z</td><td>a</td><td class="has-text-align-left" data-align="left">b </td></tr><tr><td>c</td><td>d</td><td>e</td><td>f</td><td>g</td><td>h</td><td>i</td><td>j</td><td>k</td><td class="has-text-align-left" data-align="left">l </td></tr><tr><td>m</td><td>n</td><td>o</td><td>p</td><td>q</td><td>r</td><td>s</td><td>t</td><td>u</td><td class="has-text-align-left" data-align="left">v </td></tr><tr><td>w</td><td>x</td><td>y</td><td>z</td><td>Â</td><td>À</td><td>Á</td><td>Ã</td><td>Ä</td><td class="has-text-align-left" data-align="left">Æ </td></tr><tr><td>Ç</td><td>È</td><td>É</td><td>Ê</td><td>Ë</td><td>Ì</td><td>Í</td><td>Î</td><td>Ï</td><td class="has-text-align-left" data-align="left">Ñ </td></tr><tr><td>Ò</td><td>Ó</td><td>Ô</td><td>Õ</td><td>Ö</td><td>Ù</td><td>Ú</td><td>Û</td><td>Ü</td><td class="has-text-align-left" data-align="left">ẞ </td></tr><tr><td>ß</td><td>à</td><td>á</td><td>â</td><td>ã</td><td>ä</td><td>æ</td><td>ç</td><td>è</td><td class="has-text-align-left" data-align="left">é </td></tr><tr><td>ê</td><td>ë</td><td>ì</td><td>í</td><td>î</td><td>ï</td><td>ñ</td><td>ò</td><td>ó</td><td class="has-text-align-left" data-align="left">ô </td></tr><tr><td>õ</td><td>ö</td><td>ù</td><td>ú</td><td>û</td><td>ü</td><td>ÿ</td><td>Œ</td><td>œ</td><td class="has-text-align-left" data-align="left">Ÿ </td></tr></tbody></table></figure>

## Conclusion

This article demonstrated how to perform OCR and convert images to text programmatically using C#. You can recognize the characters in the images containing single or multiple lines of text. Learn more about the C# OCR API from the [documentation][9].

## See Also

*   [Perform OCR on Images using C++][10]




[1]: #CSharp-OCR-Library-Installation
[2]: #Perform-OCR-on-Images-using-CSharp
[3]: #Perform-OCR-on-Image-of-Line-using-CSharp
[4]: https://products.aspose.com/ocr/net
[5]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[6]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeimage
[7]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[8]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeline
[9]: https://docs.aspose.com/display/ocrnet/Product+Overview
[10]: https://blog.aspose.com/2019/10/29/perform-ocr-on-images-in-c-applications-using-aspose.ocr-for-c/





