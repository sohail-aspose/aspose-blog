---
title: 'Convert GIF Images to PNG, JPEG, BMP, or TIFF using Java'
seoTitle: "Convert GIF Images in Java | GIF to PNG, JPEG, BMP, TIFF in Java"
description: "Use Java GIF converter API to convert GIF images. Convert GIF to PNG, JPEG, BMP and TIFF images programmatically using Java."
date: Thu, 25 Mar 2021 17:45:50 +0000
draft: false
url: /2021/03/25/convert-gif-to-png-jpeg-bmp-or-tiff-using-java/
author: Usman Aziz
summary: 'More often, [GIF][1] images are used to depict the animations. An animated GIF is a collection of frames combined together in a particular order. However, in certain cases, you have to convert GIF images to other raster image formats. For such cases, this article demonstrates **how to convert a GIF image to PNG, JPEG, BMP, and TIFF formats using Java**.'
tags: ['Convert GIF to JPEG in Java', 'Convert GIF to PNG in Java', 'GIF to BMP Conversion in Java', 'GIF to TIFF Conversion in Java', 'Java GIF Converter API']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/gif-to-image.jpg" alt="gif to image java">}}


More often, [GIF][2] images are used to depict the animations. An animated GIF is a collection of frames combined together in a particular order. However, in certain cases, you have to convert GIF images to other raster image formats. For such cases, this article demonstrates **how to convert a GIF image to PNG, JPEG, BMP, and TIFF formats using Java**.

*   [Java GIF Converter API][3]
*   [Convert GIF to PNG in Java][4]
*   [Convert GIF to JPEG in Java][5]
*   [GIF to BMP Conversion in Java][6]
*   [GIF to TIFF Conversion in Java][7]
*   [Get a Free API License][8]

**Info**: Aspose recently developed a FREE [Text to GIF Converter][9].

## Java GIF Converter API {#Java-GIF-Converter-API}

In order to convert GIF images, we'll use [Aspose.Imaging for Java][10]. It is a feature-rich image processing API that provides a high quality back and forth conversion of popular image formats. You can either [download][11] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-imaging-java</artifactId>
    <version>20.10</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert GIF to PNG in Java {#Convert-GIF-to-PNG-in-Java}

The following are the steps to convert a GIF image to PNG using Java.

*   First, create an instance of the [Image][12] class and load the GIF image using [Image.load(String)][13] method.
*   Create an instance of [PngOptions][14] class.
*   Instantiate [MultiPageOptions][15] class to specify frame(s) to be converted.
*   Use [PngOptions.setMultiPageOptions(MultiPageOptions)][16] method to set range of pages.
*   Finally, use [Image.save(String, PngOptions)][17] method to convert GIF to PNG.

The following code sample shows how to convert a GIF image to PNG using Java.

{{< gist aspose-com-gists 17961f60f01297fe54c8e815099c7c85 "gif-to-png.java" >}}

## Convert GIF to JPEG in Java {#Convert-GIF-to-JPEG-in-Java}

The following are the steps to convert GIF images to JPEG using Java.

*   First, create an instance of the [Image][18] class and load the GIF image using [Image.load(String)][19] method.
*   Create an instance of [JpegOptions][20] class.
*   Instantiate [MultiPageOptions][21] class to specify frame(s) to be converted.
*   Use [JpegOptions.setMultiPageOptions(MultiPageOptions)][22] method to set range of pages.
*   Finally, use [Image.save(String, JpegOptions)][23] method to convert GIF to JPEG.

The following code sample shows how to convert GIF images to JPEG in Java.

{{< gist aspose-com-gists 17961f60f01297fe54c8e815099c7c85 "gif-to-jpeg.java" >}}

## Convert GIF to BMP using Java {#GIF-to-BMP-Conversion-in-Java}

The following are the steps to convert GIF images to BMP using Java.

*   First, create an instance of the [Image][24] class and load the GIF image using [Image.load(String)][25] method.
*   Create an instance of [BmpOptions][26] class.
*   Instantiate [MultiPageOptions][27] class to specify frame(s) to be converted.
*   Use [BmpOptions.setMultiPageOptions(MultiPageOptions)][28] method to set range of pages.
*   Finally, use [Image.save(String, BmpOptions)][29] method to convert GIF to BMP.

The following code sample shows how to convert GIF images to BMP in Java.

{{< gist aspose-com-gists 17961f60f01297fe54c8e815099c7c85 "gif-to-bmp.java" >}}

## Convert GIF to TIFF using Java {#GIF-to-TIFF-Conversion-in-Java}

The following are the steps to convert GIF images to TIFF using Java.

*   First. create an instance of the [Image][30] class and load the GIF image using [Image.load(String)][31] method.
*   Create an instance of [TiffOptions][32] class.
*   Instantiate [MultiPageOptions][33] class to specify frame(s) to be converted.
*   Use [TiffOptions.setMultiPageOptions(MultiPageOptions)][34] method to set range of pages.
*   Finally, use [Image.save(String, TiffOptions)][35] method to convert GIF to TIFF.

The following code sample shows how to convert GIF images to TIFF in Java.

{{< gist aspose-com-gists 17961f60f01297fe54c8e815099c7c85 "gif-to-tiff.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Imaging for Java without evaluation limitations using a [temporary license][36].

## Conclusion

In this article, you have learned how to convert GIF images to [JPEG][37], [PNG][38], [BMP][39], and [TIFF][40] images using [Java][41]. You can explore other features of the API using [documentation][42]. Furthermore, in case of any confusion, you can contact us via our [forum][43].

## See Also

*   [Compress PNG, JPEG, and TIFF Images in Java][44]




[1]: https://docs.fileformat.com/image/gif/
[2]: https://docs.fileformat.com/image/gif/
[3]: #Java-GIF-Converter-API
[4]: #Convert-GIF-to-PNG-in-Java
[5]: #Convert-GIF-to-JPEG-in-Java
[6]: #GIF-to-BMP-Conversion-in-Java
[7]: #GIF-to-TIFF-Conversion-in-Java
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.app/slides/text-to-gif
[10]: https://products.aspose.com/imaging/java
[11]: https://downloads.aspose.com/imaging/java
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#load-java.lang.String-
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PngOptions
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/MultiPageOptions
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ImageOptionsBase#setMultiPageOptions-com.aspose.imaging.imageoptions.MultiPageOptions-
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#load-java.lang.String-
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/JpegOptions
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/MultiPageOptions
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ImageOptionsBase#setMultiPageOptions-com.aspose.imaging.imageoptions.MultiPageOptions-
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[24]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[25]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#load-java.lang.String-
[26]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/BmpOptions
[27]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/MultiPageOptions
[28]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ImageOptionsBase#setMultiPageOptions-com.aspose.imaging.imageoptions.MultiPageOptions-
[29]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[30]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[31]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#load-java.lang.String-
[32]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/TiffOptions
[33]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/MultiPageOptions
[34]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ImageOptionsBase#setMultiPageOptions-com.aspose.imaging.imageoptions.MultiPageOptions-
[35]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[36]: https://purchase.aspose.com/temporary-license
[37]: https://docs.fileformat.com/image/jpeg/
[38]: https://docs.fileformat.com/image/png/
[39]: https://docs.fileformat.com/image/bmp/
[40]: https://docs.fileformat.com/image/tiff/
[41]: https://docs.fileformat.com/programming/java/
[42]: https://docs.aspose.com/imaging/java/
[43]: https://forum.aspose.com/
[44]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/





