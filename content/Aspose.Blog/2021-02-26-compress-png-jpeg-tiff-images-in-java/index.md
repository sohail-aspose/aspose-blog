---
title: 'Compress PNG, JPEG, and TIFF Images in Java'
seoTitle: "Compress Images in Java | Compress PNG JPEG TIFF Images in Java"
description: "Use Java image compression API to compress PNG, JPEG, and TIFF images using Java. Use lossless image compression to reduce the image's size."
date: Fri, 26 Feb 2021 14:21:00 +0000
draft: false
url: /2021/02/26/compress-png-jpeg-tiff-images-in-java/
author: Usman Aziz
summary: 'In various scenarios, the images are compressed to reduce their file size. For this, different online or offline applications allow you to apply image compression. However, in certain cases, you may need to implement the image compression feature from within your web or desktop applications. For such cases, this article covers **how to compress images including PNG, JPEG, and TIFF programmatically using Java**.'
tags: ['compress jpeg in java', 'compress png in java', 'compress tiff in java', 'image compression in java']
categories: ['Aspose.Imaging Product Family']
---

In various scenarios, the images are compressed to reduce their file size. For this, different online or offline applications allow you to apply image compression. However, in certain cases, you may need to implement the image compression feature from within your web or desktop applications. For such cases, this article covers **how to compress images including [PNG][1], [JPEG][2], and [TIFF][3] programmatically using Java**.

*   [Java Image Compression API][4]
*   [Compress PNG Images in Java][5]
*   [Compress JPEG Images in Java][6]
*   [Apply Compression to TIFF Images in Java][7]
*   [Get a Free API License][8]

**Info**: Aspose recently developed a new online web app that allows you to [transform a set of images into a video][9]. You may also be interested in another service that can be used to compress videos by [extracting the sounds from videos][10].

## Java Image Compression API {#Java-Image-Compression-API}

[Aspose.Imaging for Java][11] is a powerful API that allows you to perform various image processing operations from within the Java applications. Furthermore, it lets you compress PNG, JPEG, and TIFF images seamlessly. In order to use the API, you can either [download][12] its JAR or install it within your Maven-based applications.

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
    <artifactId>aspose-imaging</artifactId>
    <version>20.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Compress PNG Images in Java {#Compress-PNG-Images-in-Java}

PNG format supports a lossless compression that means compressing a PNG image will reduce its file size but not the quality. For PNG images, Aspose.Imaging for Java lets you set compression levels from 0 to 9 where 0 and 9 are minimum and maximum compression levels respectively. The following are the steps to compress a PNG image using [Java][13].

*   First, load the PNG image using the [Image][14] class.
*   Create an instance of [PngOptions][15] class.
*   Set compression level using [PngOptions.setCompressionLevel(int)][16] method.
*   Finally, save the compressed PNG image using [Image.save(String, PngOptions)][17] method.

The following code sample shows how to compress a PNG image using Java.

{{< gist aspose-com-gists 62323e4e5d2dcc4d8c70610ab3b1a929 "compress-png.java" >}}

## Compress JPEG Images using Java {#Compress-JPEG-Images-in-Java}

For JPEG image compression, Aspose.Imaging for Java provides the following compression types.

*   Baseline
*   Progressive
*   Lossless
*   JpegLs

The following are the steps to apply one of the above-mentioned compression types to JPEG images using Java.

*   First, load the JPEG image using the [Image][18] class.
*   Create an instance of [JpegOptions][19] class.
*   Set compression level using [JpegOptions.setCompressionType(JpegCompressionMode)][20] method.
*   Finally, save the compressed JPEG image using [Image.save(String, JpegOptions)][21] method.

The following code sample shows how to compress JPEG images using Java.

{{< gist aspose-com-gists 62323e4e5d2dcc4d8c70610ab3b1a929 "compress-jpeg.java" >}}

## Compress TIFF Images using Java {#Apply-Compression-to-TIFF-Images-in-Java}

Aspose.Imaging for Java provides a variety of [TIFF compression types][22] that include LZW, Packbits, CCIT Fax 3 & 4 and etc. Therefore, you may select the compression type that best suits your requirement. The following are the steps to perform TIFF compression using Java.

*   First, load the TIFF image using the [Image][23] class.
*   Create an instance of [TiffOptions][24] class.
*   Set compression level using [TiffOptions.setCompression(TiffCompressions)][25] method.
*   Set other options such as bits per sample, photometric, palette, etc.
*   Finally, save the compressed TIFF image using [Image.save(String, TiffOptions)][26] method.

The following code sample shows how to compress TIFF images using Java.

{{< gist aspose-com-gists 62323e4e5d2dcc4d8c70610ab3b1a929 "compress-tiff.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][27].

## Conclusion

Image compression is often required in order to reduce the size of the images. Therefore, this article covered how to compress PNG, JPEG, and TIFF images programmatically using Java. Furthermore, you can explore more about the Java image processing API using [documentation][28].

## See Also

*   [Add Watermark to Images using Java][29]
*   [Convert JPG Images to PNG in Java][30]




[1]: https://docs.fileformat.com/image/png/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/tiff/
[4]: #Java-Image-Compression-API
[5]: #Compress-PNG-Images-in-Java
[6]: #Compress-JPEG-Images-in-Java
[7]: #Apply-Compression-to-TIFF-Images-in-Java
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.app/slides/video/images-to-video
[10]: https://products.aspose.app/slides/video/mp4-to-mp3
[11]: https://products.aspose.com/imaging/java
[12]: https://downloads.aspose.com/imaging/java
[13]: https://docs.fileformat.com/programming/java/
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PngOptions
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PngOptions#setCompressionLevel-int-
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/JpegOptions
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/JpegOptions#setCompressionType-int-
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.tiff.enums/TiffCompressions
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[24]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/TiffOptions
[25]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/TiffOptions#setCompression-int-
[26]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/imaging/java/
[29]: https://blog.aspose.com/2021/01/27/Add-Watermark-to-Images-using-Java/
[30]: https://blog.aspose.com/2021/11/01/convert-jpg-to-png-in-java/





