---
title: 'Convert RGB Images to Grayscale in Java'
seoTitle: "Convert RGB Image to Grayscale in Java | Binarization and Grayscaling"
description: "Use Java image processing API to convert RGB images to grayscale using Java. Use binarization methods to convert colored images to black and white."
date: Fri, 06 Aug 2021 13:41:00 +0000
draft: false
url: /2021/08/06/convert-rgb-images-to-grayscale-in-java/
author: Usman Aziz
summary: 'In various cases, you may need to convert the RGB images to grayscale or black and white, for example, in image processing, etc. In accordance with that, in this article, you will learn **how to convert an RGB image to grayscale using Java**. Moreover, the article will cover grayscaling and binarization of the images explicitly.'
tags: ['Convert Images to Black and White with Binarization Java', 'Convert Images to Grayscale in Java', 'Java API for Converting Images to Grayscale']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Convert-Image-to-Grayscale.jpg" alt="RGB image to grayscale java">}}


In various cases, you may need to convert the RGB images to grayscale or black and white, for example, in image processing, etc. In accordance with that, in this article, you will learn **how to convert an RGB image to grayscale using Java**. Moreover, the article will cover grayscaling and binarization of the images explicitly.

*   [Java API for Converting Images to Grayscale][1]
*   [Convert Images to Grayscale in Java][2]
*   [Convert Images to Black and White with Binarization][3]
    *   [Binarization with Fixed Threshold][4]
    *   [Binarization with Otsu Threshold][5]

## Java API to Convert Image to Grayscale {#API-for-Converting-Image-to-Grayscale}

In order to convert RGB images to grayscale, we'll use [Aspose.Imaging for Java][6]. It is a Java image processing API that allows you to manipulate popular image formats seamlessly. You can either [download][7] the API or install it using the following Maven configurations.

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
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert an Image to Grayscale in Java {#Convert-Image-to-Grayscale}

The following are the steps to convert an RGB image to grayscale in Java.

*   First, load the image using the [Image][8] class.
*   Then, cast the image into a [RasterCachedImage][9] object.
*   Cache the image using [RasterCachedImage.cacheData()][10] method.
*   Convert image to grayscale using [RasterCachedImage.grayscale()][11] method.
*   Finally, save the image using [RasterCachedImage.save(String)][12] method.

The following code sample shows how to convert an image to grayscale using Java.

{{< gist aspose-com-gists fdfaa4f8414fb753527a39f837ccee00 "convert-rgb-image-to-grayscale.java" >}}

### Input Image

The following is a sample image used in this article.



{{< figure align=center src="images/aspose.jpg" alt="image to grayscale Java">}}


### Converted to Grayscale

The following is the image after conversion to grayscale.



{{< figure align=center src="images/Grayscaling_out.png" alt="grayscale image">}}


## Convert Image to Black and White with Binarization {#Convert-Image-to-Grayscale-with-Binarization}

In binarization, each pixel in an image can have only two possible values; 0 or 1. Here, 0 denotes the absence and 1 denotes the presence of the color. Aspose.Imaging supports two binarization methods i.e. binarization with fixed and binarization with Otsu threshold.

### Binarization with Fixed Threshold in Java {#Binarization-with-Fixed-Threshold}

The following are the steps to perform binarization on an image using fixed threshold.

*   First, load the image using the [Image][13] class.
*   Then, cast the image into a [RasterCachedImage][14] object.
*   Cache the image using [RasterCachedImage.cacheData()][15] method.
*   Convert image to black and white using [RasterCachedImage.binarizeFixed()][16] method.
*   Finally, save the image using [RasterCachedImage.save(String)][17] method.

The following Java code applies binarization to an image and converts it to black and white.

{{< gist aspose-com-gists fdfaa4f8414fb753527a39f837ccee00 "convert-image-to-binary-fixed.java" >}}

### Binarization with Otsu Threshold in Java {#Binarization-with-Otsu-Threshold}

The following are the step to convert an image to black and white with Otsu threshold.

*   First, load the image using the [Image][18] class.
*   Cast the image into a [RasterCachedImage][19] object.
*   Cache the image using [RasterCachedImage.cacheData()][20] method.
*   Convert image to black and white using [RasterCachedImage.binarizeOtsu()][21] method.
*   Finally, save the image using [RasterCachedImage.save(String)][22] method.

The following code sample shows how to convert an image to black and white with Otsu threshold using Java.

{{< gist aspose-com-gists fdfaa4f8414fb753527a39f837ccee00 "convert-image-to-binary-otsu.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][23] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert an image to grayscale and black and white using Java. Moreover, you have seen how to apply binarization to the images with fixed or Otsu threshold. In addition, you can explore more about the Java image processing API using [documentation][24]. Also, you can share your queries with us via our [forum][25].

## See Also

*   [Compress PNG, JPEG, and TIFF Images in Java][26]
*   [Add Watermark to Images using Java][27]




[1]: #API-for-Converting-Image-to-Grayscale
[2]: #Convert-Image-to-Grayscale
[3]: #Convert-Image-to-Grayscale-with-Binarization
[4]: #Binarization-with-Fixed-Threshold
[5]: #Binarization-with-Otsu-Threshold
[6]: https://products.aspose.com/imaging/java
[7]: https://downloads.aspose.com/imaging/java
[8]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[9]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage
[10]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#cacheData--
[11]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#grayscale--
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#save-java.lang.String-
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#cacheData--
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#binarizeFixed-byte-
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#save-java.lang.String-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#cacheData--
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterCachedImage#binarizeOtsu--
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#save-java.lang.String-
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/imaging/java
[25]: https://forum.aspose.com/
[26]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/
[27]: https://blog.aspose.com/2021/01/27/add-watermark-to-images-using-java/





