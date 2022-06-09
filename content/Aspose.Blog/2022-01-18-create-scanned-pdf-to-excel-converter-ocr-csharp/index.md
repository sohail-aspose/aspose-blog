---
title: 'Create Scanned PDF to Excel Converter with OCR using C#'
seoTitle: "Create Scanned PDF to Excel Converter with OCR using C# .NET"
description: "Create Scanned PDF file to Excel Converter with OCR using C# programmatically in .NET. Convert Scanned PDF to searchable XLS or XLSX file in .NET."
date: Tue, 18 Jan 2022 09:47:00 +0000
draft: false
url: /2022/01/18/create-scanned-pdf-to-excel-converter-ocr-csharp/
author: Farhan Raza
summary: 'Scanned PDF files contain data in image format and sometimes you may need information from such documents. In certain situations, a scanned PDF file can contain numeric information which may need to be manipulated in Excel. In accordance with that, you can perform OCR operations and create an Excel file. This article covers how to **create a scanned PDF to Excel converter with OCR feature programmatically using C#.**'
tags: ['Convert Scanned PDF to Excel in csharp', 'Scanned PDF to Excel', 'Scanned PDF to Excel Converter', 'Scanned PDF to Excel OCR', 'Scanned PDF to Excel in C#']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Scanned-PDF-to-Excel-OCR.jpg" alt="Scanned PDF to Excel OCR">}}


Scanned [PDF][1] files contain data in image format and sometimes you may need information from such documents. In certain situations, a scanned PDF file can contain numeric information which may need to be manipulated in Excel. In accordance with that, you can perform OCR operations and create an Excel file. This article covers how to create a scanned PDF to Excel converter with OCR feature programmatically using C#.

*   [Create Scanned PDF to Excel Converter with OCR – C# API Installation][2]
*   [Convert Scanned PDF to Excel Programmatically in C#][3]

## Create Scanned PDF to Excel Converter with OCR – C# API Installation {#section1}

You can work with OCR features offered by the [Aspose.OCR for .NET][4] API. You can easily create a scanned PDF to Excel converter with OCR by downloading the DLL file from the [New Releases][5] section, or with the [NuGet][6] installation command below:

```
PM> Install-Package Aspose.OCR
```

## Convert Scanned PDF to Excel Programmatically in C# {#section2}

You can convert a scanned PDF document to an Excel file with OCR by following the steps below:

1.  Instantiate [AsposeOcr][7] class object.
2.  Specify a [DocumentRecognitionSettings][8] class object.
3.  Recognize the scanned PDF file with [RecognizePdf][9] method.
4.  Save output Excel file using [SaveMultipageDocument][10] method.

The following code sample explains how to convert a scanned PDF to Excel using C#:

{{< gist aspose-com-gists 17af428e962811d0b8aa74312b955115 "Scanned-PDF-to-Excel.cs" >}}

## Get Free Evaluation License

You can evaluate the feature of converting scanned PDF to Excel in its full capacity by requesting a [free temporary license][11].

## Conclusion

In this article, you have checked how to convert a scanned PDF file to Excel by applying OCR operations to recognize the text optically. This can be helpful in scenarios like when a CSV file is scanned by a scanner and a PDF file is produced. You can convert it to an Excel file programmatically using C#. Furthermore, you can take a look at other OCR-related features offered by the API by going through the [documentation][12]. In case of any queries, please feel free to contact us at the [forum][13].

## See Also

[Convert Image to Text using C# OCR Library][14]




[1]: https://docs.fileformat.com/pdf/
[2]: #section1
[3]: #section2
[4]: https://products.aspose.com/ocr/net
[5]: https://downloads.aspose.com/ocr/net
[6]: https://www.nuget.org/packages/Aspose.OCR
[7]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[8]: https://apireference.aspose.com/ocr/net/aspose.ocr/documentrecognitionsettings
[9]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizepdf
[10]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/savemultipagedocument
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/ocr/net/
[13]: https://forum.aspose.com/c/ocr/16
[14]: https://blog.aspose.com/2020/05/28/perform-ocr-on-images-and-scanned-documents-using-csharp-vb.net/




