---
title: 'Convert XPS to BMP, JPEG, PNG, and TIFF using Java'
seoTitle: "Convert XPS to BMP, JPEG, PNG, and TIFF using Java | XPS Converter"
description: "Use Java XPS converter API to convert XPS to BMP, JPEG, PNG, and TIFF programmatically in Java. Customize the XPS to raster image conversion."
date: Fri, 18 Dec 2020 09:49:58 +0000
draft: false
url: /2020/12/18/convert-xps-to-bmp-jpeg-png-and-tiff-using-java/
author: Usman Aziz
summary: '[XPS][1] (XML Paper Specifications) format was introduced by Microsoft that represents page layout. It uses XML tags to represent the appearance of the pages and the composition of the document. In this article, you will learn about the conversion of XPS documents to raster image formats programmatically. Particularly, the article will cover **how to convert XPS to [BMP][2], [JPEG][3], [PNG][4], and [TIFF][5] using Java**.'
tags: ['XPS Converter API', 'convert XPS to BMP in Java', 'convert XPS to JPEG in Java', 'convert XPS to PNG in Java', 'convert XPS to TIFF in Java']
categories: ['Aspose.Page Product Family']
---

[XPS][6] (XML Paper Specifications) format was introduced by Microsoft that is used to represent page layout. It uses XML tags to represent the appearance of the pages and the composition of the document. In various scenarios, you may need to convert XPS documents to other document formats. In accordance with that, in this article, you will learn about the conversion of XPS documents to raster image formats programmatically. Particularly, the article will cover **how to convert XPS to [BMP][7], [JPEG][8], [PNG][9], and [TIFF][10] using Java**.

*   [Java XPS to Image Converter API][11]
*   [Convert XPS to PNG][12]
*   [Convert XPS to JPEG][13]
*   [XPS to BMP Conversion][14]
*   [Convert XPS to TIFF][15]

## XPS to Image Converter API - Free Download {#XPS-to-Image-Converter-API}

[Aspose.Page for Java][16] is designed to work with PS, EPS, and XPS documents from within the Java applications. The API's built-in converter lets you perform high-quality conversion of XPS to raster image formats including PNG, JPEG, BMP, and TIFF images. You can either [download][17] the API's JAR or install it within your Maven-based applications.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-page</artifactId>
    <version>20.11</version>
</dependency>
```

## Convert XPS to Raster Images in Java

Aspose.Page for Java provides separate classes in order to customize the XPS to raster image conversion. For example, you can set the resolution of the output image, specify the pages you want to convert, and so on. The following is the list of the classes that you may use accordingly.

*   [PngSaveOptions][18] for XPS to PNG
*   [JpegSaveOptions][19] for XPS to JPEG
*   [BmpSaveOptions][20] for XPS to BMP
*   [TiffSaveOptions][21] for XPS to TIFF

## Convert XPS to PNG in Java {#Convert-XPS-to-PNG-in-Java}

The following are the steps to convert the XPS documents to PNG images using Aspose.XPS for Java.

*   Load the XPS document using [XpsDocument][22] class.
*   Create an instance of [PngSaveOptions][23] class to set additional options.
*   Create an instance of [ImageDevice][24] class.
*   Use [XpsDocument.save(ImageDevice, PngSaveOptions)][25] to save converted PNG image into [ImageDevice][26] object.
*   Use [ImageDevice][27] to save the image as a PNG file.

The following code sample shows how to convert XPS to PNG using Java.

{{< gist aspose-com-gists bcee4811da013bc7a78dd41af768a9d2 "Examples-src-main-java-com-aspose-page-conversion-XPStoPNG-XPStoPNG.java" >}}

## Convert XPS to JPEG in Java {#Convert-XPS-to-JPEG-in-Java}

The following are the steps to convert XPS to JPEG using Aspose.Page for Java.

*   Load the XPS document using [XpsDocument][28] class.
*   Use [JpegSaveOptions][29] class to set additional options for the converted JPEG image.
*   Create an instance of [ImageDevice][30] class.
*   Use [XpsDocument.save(ImageDevice, JpegSaveOptions)][31] to save converted JPEG image into [ImageDevice][32] object.
*   Use [ImageDevice][33] to save the image as a JPEG file.

The following code sample shows how to convert XPS to JPEG.

{{< gist aspose-com-gists bcee4811da013bc7a78dd41af768a9d2 "Examples-src-main-java-com-aspose-page-conversion-XPStoJPEG-XPStoJPEG.java" >}}

## Convert XPS to BMP in Java {#XPS-to-BMP-Conversion-in-Java}

You can convert the XPS files to BMP images in the same way you have done for PNG and JPEG. The following are the steps for it.

*   Use [XpsDocument][34] class to load the XPS document.
*   Create an instance of [BmpSaveOptions][35] class to set additional options for the converted BMP image.
*   Use [XpsDocument.save(ImageDevice, BmpSaveOptions)][36] method to save converted BMP image into an [ImageDevice][37] object.
*   Use [ImageDevice][38] to save the image as a BMP file.

The following code sample shows how to convert an XPS file to BMP.

{{< gist aspose-com-gists bcee4811da013bc7a78dd41af768a9d2 "Examples-src-main-java-com-aspose-page-conversion-XPStoBMP-XPStoBMP.java" >}}

## Convert XPS to TIFF in Java {#Convert-XPS-to-TIFF-in-Java}

The following are the steps to convert XPS document to TIFF image.

*   Use [XpsDocument][39] class to load the XPS document.
*   Create an instance of [TiffSaveOptions][40] class to set additional options for the converted TIFF image.
*   Use [XpsDocument.save(ImageDevice, TiffSaveOptions)][41] method to save converted TIFF image into an [ImageDevice][42] object.
*   Use [ImageDevice][43] to save the image as a TIFF file.

The following code sample shows how to convert XPS document to TIFF image in Java.

{{< gist aspose-com-gists bcee4811da013bc7a78dd41af768a9d2 "Examples-src-main-java-com-aspose-page-conversion-XSPtoTIFF-XSPtoTIFF.java" >}}

## Conclusion

In this article, you have learned how to convert XPS files to raster image formats using Java. The step-by-step guide, API references, and code samples have shown how to convert XPS to PNG, JPEG, TIFF, and BMP images. You can explore other features of the Java XPS API using the [documentation][44].

## See Also

*   [Convert PS/EPS and XPS to PDF and Raster Images in C++][45]




[1]: https://docs.fileformat.com/page-description-language/xps/
[2]: https://docs.fileformat.com/image/bmp/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/png/
[5]: https://docs.fileformat.com/image/tiff/
[6]: https://docs.fileformat.com/page-description-language/xps/
[7]: https://docs.fileformat.com/image/bmp/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/image/png/
[10]: https://docs.fileformat.com/image/tiff/
[11]: #XPS-to-Image-Converter-API
[12]: #Convert-XPS-to-PNG-in-Java
[13]: #Convert-XPS-to-JPEG-in-Java
[14]: #XPS-to-BMP-Conversion-in-Java
[15]: #Convert-XPS-to-TIFF-in-Java
[16]: https://products.aspose.com/page/java
[17]: https://downloads.aspose.com/page/java
[18]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PngSaveOptions
[19]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/JpegSaveOptions
[20]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/BmpSaveOptions
[21]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/TiffSaveOptions
[22]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument
[23]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PngSaveOptions
[24]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[25]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[26]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[27]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[28]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument
[29]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/JpegSaveOptions
[30]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[31]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[32]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[33]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[34]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument
[35]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/BmpSaveOptions
[36]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[37]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[38]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[39]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument
[40]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/TiffSaveOptions
[41]: https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[42]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[43]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/ImageDevice
[44]: https://docs.aspose.com/page/java/getting-started/
[45]: https://blog.aspose.com/2020/03/26/convert-postscript-ps-eps-and-xps-to-pdf-png-bmp-tiff-jpeg-in-cpp/





