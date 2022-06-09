---
title: 'Convert JPG Images to PNG in Java'
seoTitle: "Convert JPG Images to PNG in Java | Java Image Converter Library"
description: "Use Java image processing API to convert JPG images to PNG format in Java. Perform high quality conversion of JPG images to PNG programmatically."
date: Mon, 01 Nov 2021 13:23:00 +0000
draft: false
url: /2021/11/01/convert-jpg-to-png-in-java/
author: Usman Aziz
summary: '[JPG][1] is a well-known and one of the most commonly used image formats. However, JPG images lose quality each time they are saved. Therefore, you may need to convert them into a lossless format such as [PNG][2]. To perform this conversion programmatically, this article shows **how to convert a JPG image to PNG in Java**.'
tags: ['Convert a JPG to PNG in Java', 'Java API for JPG to PNG Conversion', 'Java Image converter library', 'java jpg to png converter']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/convert-jpg-to-png.jpg" alt="convert jpg images to png format in java">}}


[JPG][3] is a well-known and one of the most commonly used image formats. However, JPG images lose quality each time they are saved. Therefore, you may need to convert them into a lossless format such as [PNG][4]. To perform this conversion programmatically, this article shows **how to convert a JPG image to PNG in Java**.

*   [Java API for JPG to PNG Conversion][5]
*   [Convert a JPG Image to PNG][6]

## Java API for JPG to PNG Conversion {#API-for-JPG-to-PNG-Conversion}

[Aspose.Imaging for Java][7] is a feature-rich image processing API that supports the manipulation of popular image formats. Moreover, it lets you convert images from one format to another seamlessly. In this article, we will use this API to convert our JPG images to PNG format. You can either [download][8] the API’s JAR or install it using the following Maven configuration in **pom.xml**.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-imaging-java</artifactId>
    <version>21.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert a JPG Image to PNG in Java {#Converting-a-PNG-Image-to-JPG}

It is quite straightforward to convert a JPG image to PNG format using Aspose.Imaging. You only need to load the JPG file and save it as a PNG image. The following are the steps to convert a JPG image to PNG in Java.

*   Load the JPG file using [Image][9] class.
*   Create an instance of [PngOptions][10] class.
*   Set color type using [PngOptions.setColorType()][11] method.
*   Convert JPG image to PNG using [Image.Save(string, PngOptions)][12] method.

The following code sample shows how to convert a JPG image to PNG format.

{{< gist aspose-com-gists 39cf2f9708713e487dfa66021b888285 "jpg-to-png.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][13] to use Aspose.Imaging for Java without evaluation limitations.

## Conclusion

JPG to PNG conversion is often performed to convert images to a lossless format. In this article, you have learned how to convert JPG images to PNG format programmatically in Java. Thus, you can easily embed JPG to PNG conversion into your Java applications. In addition, you can explore Java image processing API using its [documentation][14]. Also, you can share your queries on our [forum][15].

## See Also

*   [](https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/)[Compress PNG, JPEG, and TIFF Images in Java][16]
*   [](https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/)[Add Watermark to Images using Java][17]




[1]: https://docs.fileformat.com/image/jpeg/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/png/
[5]: #API-for-JPG-to-PNG-Conversion
[6]: #Converting-a-PNG-Image-to-JPG
[7]: https://products.aspose.com/imaging/java/
[8]: https://downloads.aspose.com/imaging/java/
[9]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[10]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PngOptions
[11]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PngOptions#setColorType-int-
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/imaging/java/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/
[17]: https://blog.aspose.com/2021/01/27/add-watermark-to-images-using-java/




