---
title: 'Convert Image to Excel with OCR in C#'
date: Wed, 26 Jan 2022 10:18:00 +0000
draft: false
url: /2022/01/26/image-to-excel-ocr-csharp/
author: ''Farhan Raza''
summary: 'Images contain visual information which may be needed in text format for processing data. In such situations, **you can convert an image to Excel format programmatically in C#**. For example, an image can contain numeric values which you might need to perform calculations. In accordance with that, this article covers how to convert an image to an Excel file.'
tags: ['Image to Excel', 'Image to Excel in csharp', 'JPG to Excel in csharp', 'PNG to Excel in csharp', 'Scanned Image to Excel']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-Excel-OCR-1.jpg" alt="Image to Excel C# .NET">}}


Images contain visual information which may be needed in text format for processing data. In such situations, you can convert an image to Excel format programmatically in C#. For example, an image can contain numeric values which you might need to perform calculations. In accordance with that, this article covers how to convert an image to an Excel file.

*   [Image to Excel Converter in C# – API Installation][1]
*   [Convert Image to Excel File with OCR Programmatically using C#][2]
*   [Convert Image from URI to Excel with OCR in C#][3]

## Image to Excel Converter in C# – API Installation {#section1}

You can recognize images by performing OCR operations with [Aspose.OCR for .NET][4] API. Quickly configure the API by downloading its DLL file from the [Downloads][5] section or using [NuGet][6] package manager with the following command:

```
PM> Install-Package Aspose.OCR
```

## Convert Image to Excel File with OCR Programmatically using C# {#section2}

You can convert an image to an Excel file with OCR by following the steps below:

1.  Firstly, create an object of [AsposeOcr][7] class.
2.  Recognize the input image.
3.  Finally, save the output file in Excel format.

The code snippet below demonstrates how to convert an image to an Excel file in XLS or XLSX format programmatically using C#:

{{< gist aspose-com-gists fc8295feb215ab47140d2b068e6f6bbc "OCRImagetoExcelcsharp.cs" >}}

## Convert Image from URI to Excel with OCR in C# {#section3}

You can load the input image from an online URI and convert it to Excel format with OCR by following the steps below:

1.  Firstly, initialize an instance of [AsposeOcr][8] class.
2.  Recognize image with OCR using [RecognizeImage()][9] method.
3.  Finally, save the result as an Excel file.

The following code shows how to convert an image from URI to an Excel file programmatically with C#:

{{< gist aspose-com-gists fc8295feb215ab47140d2b068e6f6bbc "OCRuriImageToExcelcsharp.cs" >}}

## Get Free API License

You can evaluate the API in its full capacity by requesting a [free temporary license][10].

## Conclusion

In conclusion, you have learned how to convert an image from the disk or from an online URI to an Excel file with the OCR feature programmatically using C#. Moreover, you can find details about other features by taking a look at the [documentation][11]. Furthermore, please feel free to reach out to us at the [forum][12] for any of your inquiries.

## See Also

[Convert Scanned PDF to Searchable PDF with OCR in C#][13]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/ocr/net
[5]: https://downloads.aspose.com/ocr/net
[6]: https://www.nuget.org/packages/Aspose.OCR/
[7]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[8]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[9]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeimage/index
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/ocr/net/
[12]: https://forum.aspose.com/c/ocr/16
[13]: https://blog.aspose.com/2022/01/13/convert-scanned-pdf-to-searchable-csharp/




