---
title: 'Recognize Text with OCR on DjVu Image in C#'
date: Tue, 24 May 2022 09:05:06 +0000
draft: false
url: /2022/05/24/recognize-text-ocr-djvu-csharp/
author: 'Farhan Raza'
summary: 'The DjVu format is used to store scanned documents as they can include text, images, or drawings. It is used to archive data because this format is able to store the data using the minimum space. This article covers how to **recognize text from DjVu images with OCR operations programmatically in C#**.'
tags: ['C# OCR DJVU', 'DjVu Image OCR', 'OCR DjVu Image', 'Recognize text in DjVu Image']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/recognize-Text-DjVu-C-1024x536.jpg" alt="Recognize text DjVu Image C# OCR">}}


The [DjVu](https://docs.fileformat.com/image/djvu/) format is used to store scanned documents as they can include text, images, or drawings. DjVu is used to archive data because it is able to store the data using the minimum space. This article covers how to recognize text from DjVu images with OCR operations programmatically in C#.

*   [Text Recognition from DjVu Image – C# API Installation](#section1)
*   [Recognize Text by Performing OCR on DjVu Image in C#](#section2)

## Text Recognition from DjVu Image – C# API Installation {#section1}

[Aspose.OCR for .NET](https://products.aspose.com/ocr/net) API supports optical character recognition for different types of documents like JPG, PNG, PDF, etc. Likewise, it also supports text recognition from multipage DjVu image files. You can easily configure the API by downloading the JAR file of the API from the [Downloads](https://downloads.aspose.com/ocr/net) section. Likewise, you can run the following [NuGet](https://www.nuget.org/packages/Aspose.OCR/) installation command to install the library in your project:

```
PM> Install-Package Aspose.OCR
```

## Recognize Text by Performing OCR on DjVu Image in C# {#section2}

You can recognize text by performing OCR operations on multiple page DjVu images by following the steps below:

1.  Initialize an API instance using the [AsposeOCR](https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr) class.
2.  Create a [DocumentRecognitionSettings](https://apireference.aspose.com/ocr/net/aspose.ocr/documentrecognitionsettings) class object.
3.  Recognize text using the [RecognizeDjvu](https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/recognizedjvu/) method.
4.  Print the recognized text.

The following code sample shows how to recognize text from a DjVu image by performing OCR programmatically in C#:



## Get a Free API License

You can request a [Free Temporary License](https://purchase.aspose.com/temporary-license) to evaluate the API without any evaluation limitations.

## Conclusion

In conclusion, you have learned how to recognize text with OCR operations on a multi-page DjVu image. You can recognize text with the ability to specify the document recognition settings where you can set auto-contrast and skewing options for the input image in order to increase the accuracy of the text recognition process. Furthermore, you may explore various other features supported by the API by taking a look at the [documentation](https://docs.aspose.com/ocr/net/) section. In case you need to discuss any of your concerns or requirements, please feel free to write to us at the [forum](https://forum.aspose.com/c/ocr).

## See Also

[Convert Image to Excel with OCR in C#](https://blog.aspose.com/2022/01/26/image-to-excel-ocr-csharp/)




