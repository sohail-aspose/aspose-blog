---
title: 'Convert Scanned PDF File to Text in C#'
seoTitle: "Convert Scanned PDF Document to Text File Programmatically in C#"
description: "You can convert a scanned PDF document to text string or TXT file programmatically using C#. Extract text from scanned PDF file in .NET."
date: Tue, 30 Nov 2021 22:23:00 +0000
draft: false
url: /2021/11/30/scanned-pdf-to-text/
author: Farhan Raza
summary: 'A scanned PDF file is basically one or more flat images captured by a scanner or a camera. You cannot copy, paste, or process information from such files. This article covers how to **convert a scanned PDF to text in C#.**'
tags: ['Convert scanned PDF', 'Convert scanned PDF in csharp', 'scanned PDF to TXT file', 'scanned PDF to text']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/scanned-pdf-to-text-ocr.png" alt="scanned pdf to text">}}


A scanned PDF file is basically one or more flat images captured by a scanner or a camera. You cannot copy, paste, or process information from such files. This article covers how to convert a scanned PDF to text in C#.

*   [Scanned PDF to Text Converter – C# API Installation][1]
*   [Convert Scanned PDF to Text String in C#][2]
*   [Convert Scanned PDF to TXT File Programmatically in C#][3]

## Scanned PDF to Text Converter – C# API Installation {#section1}

[Aspose.OCR for .NET][4] API is used to perform OCR operations. It can recognize the characters optically from images or scanned PDF documents. Please configure the API by downloading the DLL file from the [New Releases][5] section, or with the following [NuGet][6] installation command.

```
PM> Install-Package Aspose.OCR
```

## Convert Scanned PDF to Text String in C# {#section2}

You can convert a scanned PDF file to a text string by performing OCR operations on it. You need to follow the steps below to print the text from a scanned PDF document:

1.  Specify the setting for recognizing the scanned PDF file.
2.  Initialize [AsposeOcr][7] class instance.
3.  Initialize [RecognitionResult][8] class object.
4.  Print the text after recognizing it from scanned PDF.

The following code snippet shows how to recognize text from scanned PDF in C#:

{{< gist aspose-com-gists cf2075ea56b18525c0108aeb290d6e8f "Scanned-PDF-to-Text.cs" >}}

## Convert Scanned PDF to TXT File Programmatically in C# {#section3}

You can convert a scanned PDF file to a TXT file with the following steps:

1.  Instantiate [AsposeOcr][9] class object.
2.  Create [DocumentRecognitionSettings][10] class object.
3.  Save recognition results and initialize [StringBuilder][11] class instance.
4.  Save the result in a TXT file.

The code snippet below explains how to convert a scanned PDF file to a TXT file programmatically in C#:

{{< gist aspose-com-gists cf2075ea56b18525c0108aeb290d6e8f "Scanned-PDF-to-Text-File.cs" >}}

## Get Free Evaluation License

You can request a [free evaluation license][12] to test the API in its full capacity.

## Conclusion

In this article, you have learned how to convert scanned PDF to a text string or a text file programmatically using C#. Moreover, you may check several other features of the API by visiting the [documentation][13]. Please feel free to contact us at the [forum][14] in case of any concerns.

## See Also

[Convert Image to Searchable PDF with OCR using C#][15]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/ocr/net
[5]: https://downloads.aspose.com/ocr/net
[6]: https://www.nuget.org/packages/Aspose.OCR/
[7]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[8]: https://apireference.aspose.com/ocr/net/aspose.ocr/recognitionresult
[9]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[10]: https://apireference.aspose.com/ocr/net/aspose.ocr/documentrecognitionsettings
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.text.stringbuilder?view=net-6.0
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/ocr/net/
[14]: https://forum.aspose.com/c/ocr/16
[15]: https://blog.aspose.com/2021/06/04/convert-image-to-searchable-pdf-with-ocr-using-csharp/




