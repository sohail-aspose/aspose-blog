---
title: 'Resize Images Programmatically in Java'
seoTitle: "Resize Images in Java | Java Image Resizer for PNG, JPG, GIF, SVG"
description: "Use Java image processing API to resize images in Java. Resize raster or vector images using different resizing techniques. Resize image proportionally."
date: Mon, 22 Nov 2021 12:03:00 +0000
draft: false
url: /2021/11/22/resize-images-in-java/
author: Usman Aziz
summary: 'The [image editors][1] provide resizing feature that lets you alter the size of images as per your requirements. While designing an image editor or processing images from within your Java applications, you may need to resize images programmatically. To accomplish that, this article covers **how to resize images in Java**. Moreover, you will also learn how to resize images using different resizing techniques.'
tags: ['Java API to Resize Images', 'Java Image Editor Library', 'Java Image Resizer API', 'Resize Raster Images in Java', 'Resizing Vector Images in Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Resize-images.jpg" alt="Resize image using Java image resizer">}}


The [image editors][2] provide resizing feature that lets you alter the size of images as per your requirements. While designing an image editor or processing images from within your Java applications, you may need to resize images programmatically. To accomplish that, this article covers **how to resize images in Java**. Moreover, you will also learn how to resize images using different resizing techniques.

*   [Java API to Resize Images][3]
*   [Resize Raster Images][4]
    *   [Simple Resizing of an Image][5]
    *   [Resize an Image using a Particular Type][6]
    *   [Resize Image Proportionally][7]
*   [Resizing Vector Images][8]

## Java API to Resize Images {#API-to-Resize-Images}

[Aspose.Imaging for Java][9] is a widely used image processing API that lets you manipulate images quite easily. We will use this API to resize images in this article. You can download the API from the [downloads section][10]. Also, you can install it from Maven using the following configuration in **pom.xm**l.

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

## Resize Raster Images in Java {#Reszie-Raster-Images}

Aspose.Imaging for Java provides two ways to resize raster images. One is simple resizing in which you provide the height and width of the resultant image. Whereas, in the second method, you also specify a resize type that tells the API about the resizing technique that should be used, such as Lanczos Resampling, Nearest Neighbor Resampling, etc. In the following sections, we will discuss how to implement each of these methods to resize images.

### Resize an Image with Simple Resizing {#Simple-Resizing-of-an-Image}

In this resizing method, you only have to provide the dimensions of the resultant image. The following are the steps to resize an image in Java.

*   First, use [Image][11] class to load the image you want to resize.
*   Then, call [Image.resize(int, int)][12] method to resize the image.
*   Finally, save the resultant image using [Image.save(string)][13] method.

The following code snippet resizes an image to the provided height and width.

{{< gist aspose-com-gists 61c3c13a1fd754417756a75da7690acb "resize-image.java" >}}

### Resize Image using a Resize Type {#Resize-an-Image-using-ResizeType-Enum}

Aspose.Imaging for Java provides a wide range of resizing techniques, which are listed [here][14]. You can choose one that suits your scenario. For example, **Lanczos Resampling** is recommended for quality image resizing, however, it works slower. Whereas, for fast resizing **Nearest Neighbour Resampling** is used, however, it compromises the quality of the image. The following are the steps to resize an image using a particular resize technique.

*   First, use [Image][15] class to load the image you want to resize.
*   Then, call [Image.resize(int, int, ResizeType)][16] method to resize the image using a particular technique.
*   Finally, save the resultant image using [Image.save(string)][17] method.

The following code sample shows how to resize an image using a particular resizing technique.

{{< gist aspose-com-gists 61c3c13a1fd754417756a75da7690acb "resize-image-type.java" >}}

### Proportional Image Resizing in Java {#Resize-Image-Proportionally}

The aspect ratio is calculated while resizing the images to avoid shrunk or scaled resultant images. However, any miscalculation of the aspect ratio may cause stretched images. To get rid of such issues, you can let the API take care of the aspect ratio itself. The following are the steps to resize an image proportionally.

*   First, use [Image][18] class to load the image you want to resize.
*   Cache image data using [Image.cacheData()][19] method.
*   Define height and width of the resultant image.
*   Call [Image.resizeWidthProportionally(int)][20] and [Image.resizeHeightProportionally(int)][21] methods to calculate proportion values.
*   Finally, save the resultant image using [Image.save(string)][22] method.

You can also specify a particular resize type while resizing the image proportionally using the overload [Image.resizeWidthProportionally(int, ResizeType)][23] and [Image.resizeHeightProportionally(int, ResizeType)][24] methods.

The following Java code sample shows how to resize an image proportionally.

{{< gist aspose-com-gists 61c3c13a1fd754417756a75da7690acb "resize-image-proportionally.java" >}}

## Resizing Vector Images in Java {#Resize-Vector-Images}

You can also resize a vector image and save it to a raster image format such as PNG, JPEG, GIF, etc. The following code demonstrates how to achieve that in Java using Aspose.Imaging.

{{< gist aspose-com-gists 61c3c13a1fd754417756a75da7690acb "resize-vector-image.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Imaging for Java without evaluation limitations by getting a [free temporary license][25].

## Conclusion

In this article, you have learned how to resize images programmatically in Java. Furthermore, the article has covered how to resize images using different techniques such as Lanczos Resampling, Nearest Neighbor Resampling, etc. In addition, proportional image resizing and resizing of vector images are also discussed. You can visit [documentation][26] to read more about Java image processing API. Also, you can learn from the source code samples available on [GitHub][27]. In case of any questions, you can reach us at our [forum][28].

## See Also

*   [Compress PNG, JPEG, and TIFF Images in Java][29]
*   [Add Watermark to Images using Java][30]




[1]: https://en.wikipedia.org/wiki/Image_editing#Image_editor_features
[2]: https://en.wikipedia.org/wiki/Image_editing#Image_editor_features
[3]: #API-to-Resize-Images
[4]: #Reszie-Raster-Images
[5]: #Simple-Resizing-of-an-Image
[6]: #Resize-an-Image-using-ResizeType-Enum
[7]: #Resize-Image-Proportionally
[8]: #Resize-Vector-Images
[9]: https://products.aspose.com/imaging/java/
[10]: https://downloads.aspose.com/imaging/java/
[11]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resize-int-int-
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ResizeType
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resize-int-int-int-
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#cacheData--
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeWidthProportionally-int-
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeHeightProportionally-int-
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeWidthProportionally-int-int-
[24]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#resizeHeightProportionally-int-int-
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/imaging/java/
[27]: https://github.com/aspose-imaging/Aspose.Imaging-for-Java
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/
[30]: https://blog.aspose.com/2021/01/27/add-watermark-to-images-using-java/




