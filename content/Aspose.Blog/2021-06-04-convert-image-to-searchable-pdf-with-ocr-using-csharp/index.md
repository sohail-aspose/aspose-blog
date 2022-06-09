---
title: 'Convert Image to Searchable PDF with OCR using C#'
seoTitle: "Convert JPG PNG TIFF Image to Searchable PDF with OCR using C#"
description: "Convert JPG PNG TIFF BMP and other image formats to searchable PDF files by OCR. Convert scanned documents to searchable PDF Programmatically in C# .NET."
date: Fri, 04 Jun 2021 11:54:00 +0000
draft: false
url: /2021/06/04/convert-image-to-searchable-pdf-with-ocr-using-csharp/
author: Farhan Raza
summary: 'Images or scanned documents can contain textual information. You can **convert a scanned document or an image to a searchable PDF document with OCR programmatically using C#**. So the JPG, PNG, TIFF, BMP, and other format images can be converted to searchable PDF files. Please refer to the following sections for further details.'
tags: ['Image to PDF', 'Image to PDF conversion', 'Image to Searchable PDF', 'Image to Text PDF', 'JPG to Searchable PDF Csharp', 'Scanned Documents to PDF']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-PDF-OCR-in-C.png" alt="Image to PDF OCR">}}


Images or scanned documents can contain textual information. You can convert a scanned document or an image to a searchable [PDF][1] document with OCR programmatically using C#. So the [JPG][2], [PNG][3], [TIFF][4], [BMP][5], and other [image formats][6] can be converted to searchable PDF files. Please refer to the following sections for further details:

*   [Image to Searchable PDF Converter with OCR – C# API Installation][7]
*   [Convert Image to Searchable PDF with OCR Programmatically using C#][8]
*   [Convert Skewed Image to Searchable PDF with OCR Programmatically in C#][9]

## Image to Searchable PDF Converter with OCR – C# API Installation {#section1}

[Aspose.OCR for .NET][10] API can efficiently perform OCR operations on images or scanned documents. You can configure the API by downloading the DLL file from the [New Releases][11] section, or with the following [NuGet][12] installation command:

```
PM> Install-Package Aspose.OCR
```

## Convert Image to Searchable PDF with OCR Programmatically using C# {#section2}

You can convert a JPG, PNG, TIFF and other image formats to a searchable PDF with OCR by following the steps below:

1.  Set path for input image to recognize.
2.  Initialize [AsposeOcr][13] class instance.
3.  Recognize input image with [RecognizeImage][14] method.
4.  Save output to searchable PDF file.

The code below shows how to convert JPG, PNG, TIFF, and other image formats to searchable PDF with OCR using C#:

{{< gist aspose-com-gists 116dd2536967d784fb63cebcc96f2ec3 "Image-to-PDF-OCR.cs" >}}

## Convert Skewed Image to Searchable PDF with OCR Programmatically in C# {#section3}

Images can sometimes be skewed for different reasons. Sometimes you may know the skew angle of the images and specify it before recognizing the image, however, you can calculate the skew angle with the API when you do not know the angle. The following steps show how to convert a skewed image to a searchable PDF file:

1.  Specify the path for input image.
2.  Initialize [AsposeOcr][15] class object.
3.  Initialize [RecognitionSettings][16] class instance.
4.  Calculate the skew angle of the image.
5.  Recognize the image and save output searchable PDF file.

The following code shows how to convert a skewed image to searchable PDF file programmatically using C#:

{{< gist aspose-com-gists 116dd2536967d784fb63cebcc96f2ec3 "Image-to-PDF-Skew.cs" >}}

Below is a screenshot of the input image and output PDF file:



{{< figure align=center src="images/Image-to-PDF-OCR-1024x475.png" alt="Image to PDF OCR">}}


## Get Free Evaluation License

You can evaluate the API without any limitations by requesting a [Free Temporary License][17].

## Conclusion

In this article, you have explored how to convert an image to a searchable PDF file programmatically using C#. A JPG, PNG, BMP, TIFF as well as a scanned document can be converted to a PDF file. You can explore other features of the API by visiting the [Documentation][18] section and feel free to contact us at [Free Support Forum][19] for any of your concerns.

## See Also

[Convert Image to Word Document (DOCX) with OCR using C#][20]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/tiff/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/image/
[7]: #section1
[8]: #section2
[9]: #section3
[10]: https://products.aspose.com/ocr/net
[11]: https://downloads.aspose.com/ocr/net
[12]: https://www.nuget.org/packages/Aspose.OCR/
[13]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[14]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr/methods/recognizeimage/index
[15]: https://apireference.aspose.com/ocr/net/aspose.ocr/asposeocr
[16]: https://apireference.aspose.com/ocr/net/aspose.ocr/recognitionsettings
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/ocr/net/
[19]: https://forum.aspose.com/c/ocr/16
[20]: https://blog.aspose.com/2021/05/19/image-to-word-docx-ocr-csharp/





