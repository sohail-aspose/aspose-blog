---
title: 'Convert JPG, PNG, TIFF, EMF, or BMP Images to PDF using C#'
seoTitle: "C# Convert Images to PDF | Convert JPG, PNG, TIFF, EMF, BMP to PDF"
description: "Convert images to PDF in C# .NET. JPG, PNG, TIFF, EMF, and BMP to PDF in Windows/Mac. Create, Change, Make & Save photo or (pic) picture to PDF high quality."
date: Sun, 26 Jul 2020 22:27:18 +0000
draft: false
url: /2020/07/26/images-to-pdf-csharp/
author: Farhan Raza
summary: ''
tags: ['Convert Tiff to PDF', 'Image to PDF', 'add picture to pdf', 'bmp to pdf', 'emf to pdf', 'jpg to pdf', 'jpg to pdf high quality', 'jpg2pdf', 'konvert jpg ke pdf', 'photo to pdf', 'pic to pdf', 'picture to pdf', 'png to pdf', 'save jpg as pdf', 'tiff to pdf']
categories: ['Aspose.PDF Product Family']
---

Images to PDF conversion is an important and useful scenario for file processing applications. In this article, we will be learning to convert JPG, PNG, TIFF, EMF, WMF, and BMP images to PDF conversion using C# or VB.NET. The following are the installation steps and a few of the possible use cases for converting images:

*   [JPG, PNG, TIFF, EMF, and BMP to PDF Converter API - Installation][1]
*   [Convert JPG to PDF with C#][2]
*   [Convert Image to PDF with Same Page Height and Width in C#][3]
*   [Convert PNG to PDF using C#][4]
*   [Convert TIFF to PDF using C#][5]
*   [Convert EMF Image to PDF using C#][6]
*   [Convert BMP to PDF with C#][7]

## C# Image to PDF Converter API - Installation {#new}

We will be performing these image formats to PDF conversion using [Aspose.PDF for .NET][8] API. You can either download it from [Releases][9] section, or via the [NuGet Gallery][10] with the following command:

```
_Install-Package Aspose.Pdf -Version 20.9.0_
```

So the API has been installed successfully by now. Let us move on to explore different use cases:

## Convert JPG to PDF with C# {#section1}

You can easily convert a [JPG][11] image to PDF by following steps:

1.  Initialize object of Document class
2.  Add a new Page to PDF document
3.  Load JPG image and add to paragraph
4.  Save output PDF

The code snippet below shows how to convert JPG Image to PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Image-to-PDF.cs" >}}

Below is the screenshot of JPG conversion to PDF:



{{< figure align=center src="images/Image-To-PDF.png" alt="Image to PDF">}}


However, in this screenshot, you can notice that the image is converted to a PDF page, but, default page dimensions and margins are applied in the output PDF document. [Aspose.PDF for .NET][12] API allows you to control page dimensions and margin that help you create exactly the same size PDF as of the image dimensions. Let us proceed to explore this feature:

## Convert Image to PDF with Same Page Height and Width {#section2}

Continuing this example from the above use case, as you can notice bigger page size in the above screenshot. Let us learn how to convert an image to PDF with the same height and width of the page. We will be getting the image dimensions and accordingly set the page dimensions of PDF document with the below steps:

1.  Load input image file
2.  Get the height and width of the image
3.  Set height, width, and margins of a page
4.  Save the output PDF file

Following code snippet shows how to convert an **Image to PDF** with same page height and width using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "JPG-to-PDF.cs" >}}

So you can notice the difference of page dimensions that have been created with updated code snippet:



{{< figure align=center src="images/JPG-to-PDF-1024x648.png" alt="">}}


Finally, you can notice the page size is exactly similar in accordance with input image dimensions, and there are no more default page margins being set now.

## Convert PNG to PDF using C# {#section3}

[PNG][13] image format is popular because of its features as compared to JPG images. For example, PNG images support transparency. Firstly, let us convert PNG to PDF with below steps:

1.  Load input PNG image
2.  Read height and width values
3.  Create new document and add Page
4.  Set page dimensions
5.  Save output file

Moreover, the code snippet below shows how to convert PNG to PDF with C# in your .NET applications:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PNG-to-PDF.cs" >}}

## Convert TIFF to PDF using C# {#section4}

A [TIFF][14] image is different from conventional JPEG, PNG, or other formats in a way that a TIFF image can contain several frames with different images. Aspose.PDF file format is also supported, be it a single frame or multi-frame TIFF image. So you can convert the TIFF image to PDF in your .NET applications. Therefore, we will consider an example of converting multi-page TIFF image to multi-page PDF document with below steps:

1.  Instantiate an instance of [Document][15] class
2.  Load input TIFF image
3.  Get FrameDimension of the frames
4.  Add new page for each frame
5.  Finally, save images to PDF pages

Moreover, the following code snippet shows how to convert multi-page or multi-frame TIFF image to PDF with C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "TIFF-to-PDF.cs" >}}

## Convert EMF Image to PDF using C# {#section5}

[EMF][16] images, also known as **Enhanced Metafile Format**, are actually device-independent images. Furthermore, you can convert EMF to PDF image using the below steps:

1.  Firstly, initialize [Document][17] class object
2.  Load EMF image file
3.  Add the loaded EMF image to a Page
4.  Save PDF document

Moreover, the following code snippet shows how to convert an EMF to PDF with C# in your .NET code snippet:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "EMF-to-PDF.cs" >}}

## Convert BMP to PDF with C# {#section6}

[BMP][18] images are Bitmap images that you can convert to PDF with Aspose.PDF for .NET API. Therefore, you can follow the following steps to convert BMP images:

1.  Initialize a new Document
2.  Load input BMP image
3.  Finally, save the output PDF file

So the following code snippet follows these steps and shows how to convert BMP to PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "BMPtoPDF.cs" >}}

## Conclusion

After all, we have explored images to PDF conversion from different aspects using C#. Different conversions including JPG, PNG, TIFF, EMF, and BMP to PDF conversion has been discussed in detail. Moreover, we have learned how to improve the image to PDF rendering while setting page size and margins. Furthermore, if you still have any inquiries or questions then please reach out to us at [Free Support Forum][19].

## See Also

[Convert AI to PNG, JPG, PSD and PDF file with C# .NET][20]




[1]: #new
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: #section6
[8]: https://products.aspose.com/pdf/net
[9]: https://releases.aspose.com/
[10]: https://www.nuget.org/packages/Aspose.Pdf
[11]: https://docs.fileformat.com/image/jpeg/
[12]: https://products.aspose.com/pdf/net
[13]: https://docs.fileformat.com/image/png/
[14]: https://docs.fileformat.com/image/tiff/
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://docs.fileformat.com/image/emf/
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[18]: https://docs.fileformat.com/image/bmp/
[19]: https://forum.aspose.com/c/pdf
[20]: https://blog.aspose.com/2020/07/01/convert-ai-to-png-jpg-psd-and-pdf-csharp/





