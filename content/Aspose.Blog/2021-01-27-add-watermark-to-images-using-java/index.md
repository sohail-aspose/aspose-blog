---
title: 'Add Watermark to Images using Java'
seoTitle: "Add Watermark to Images using Java | PNG, JPEG, BMP, and Others"
description: "Use Java image processing API to add watermark to images using Java. Add watermark to PNG, JPEG, BMP and other popular image formats in Java."
date: Wed, 27 Jan 2021 03:44:00 +0000
draft: false
url: /2021/01/27/add-watermark-to-images-using-java/
author: Usman Aziz
summary: 'Watermark is a convenient way of protecting the content and claiming the copyrights. By applying a watermark to digital documents or images, you can avoid unauthorized usage or theft. In accordance with that, this article covers how to automate watermarking feature for images within Java applications. Particularly, you will learn **how to add watermark to images using Java**. This can be useful especially when you need to add a watermark to a batch of images.'
tags: ['Add-Diagonal-Watermark-to-images-in-Java', 'Add-Watermark-to-an-Image-in-Java', 'Java-API-to-Add-Watermark-to-Images']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Images.jpg" alt="Add watermark to images in Java">}}


Watermark is a convenient way of protecting the content and claiming the copyrights. By applying a watermark to digital documents or images, you can avoid unauthorized usage or theft. In accordance with that, this article covers how to automate watermarking feature for images within [Java][1] applications. Particularly, you will learn **how to add watermark to images using Java**. This can be useful especially when you need to add a watermark to a batch of [images][2].

*   [Java API to Add Watermark to Images][3]
*   [Add Watermark to an Image in Java][4]
*   [Add Diagonal Watermark to images in Java][5]
*   [Get Free API License][6]

## Java API to Add Watermark to Images {#Java-API-to-Add-Watermark-to-Images}

In order to add a watermark to images, we'll use [Aspose.Imaging for Java][7]. It is an image processing API that lets you manipulate a wide range of image formats from within your Java applications. You can either [download][8] the API's JAR or install it within your Maven-based applications using the following configurations.

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

## Add Watermark to Images using Java {#Add-Watermark-to-Images-in-Java}

The following are the steps to add a watermark to the images using Aspose.Imaging.

*   Load an image file using the [Image][9] class.
*   Create an object of the [Graphics][10] class and initialize it with _Image_ object.
*   Create and initialize [Font][11] and [SolidBrush][12] objects.
*   Add watermark using [Graphics.drawString(String s, Font font, Brush brush, float x, float y)][13] method.
*   Save the image using [Image.save()][14] method.

The following code sample shows how to add watermark to an image using Java.

{{< gist aspose-com-gists 013c207eaf0c3750e9c31c38a8d14100 "add-watermark-to-image.java" >}}

## Add Diagonal Watermark to images in Java {#Add-Diagonal-Watermark-to-images-in-Java}

In certain cases, the watermark is applied to the images diagonally. For such cases, Aspose.Imaging for Java provides watermark transformation options using which you can rotate the watermark. The following are the steps to add a diagonal watermark to an image.

*   Load an image file using the [Image][15] class.
*   Create an object of the [Graphics][16] class and initialize it with _Image_ object.
*   Create and initialize [Font][17] and [SolidBrush][18] objects.
*   Get image size in the [Size][19] object.
*   Create a new [Matrix][20] object and set translation and transformation to the desired angle.
*   Use [Graphics.setTransform(Matrix)][21] method to set transformation of the watermark.
*   Add watermark using [Graphics.drawString(String s, Font font, Brush brush, float x, float y)][22] method.
*   Save the image using [Image.save()][23] method.

The following code sample shows how to add a diagonal watermark to image using Java.

{{< gist aspose-com-gists 013c207eaf0c3750e9c31c38a8d14100 "add-diagonal-watermark-to-image.java" >}}

## Get a Free API License {#Get-a-Free-License}

You can [get a free temporary license][24] in order to try the API without evaluation limitations.

## Conclusion

Watermark is used to protect digital documents and images from unauthorized or illegal usage. In order to protect digital images, this article covered how to add a watermark to images using Java. Furthermore, you have seen how to apply the transformation to the watermarks. You can explore more about the Java image processing API using the [documentation][25].

## See Also

*   [Convert DICOM to JPEG, GIF, PNG, BMP and PDF in Java][26]




[1]: https://docs.fileformat.com/programming/java/
[2]: https://docs.fileformat.com/image/
[3]: #Java-API-to-Add-Watermark-to-Images
[4]: #Add-Watermark-to-Images-in-Java
[5]: #Add-Diagonal-Watermark-to-images-in-Java
[6]: #Get-a-Free-License
[7]: https://products.aspose.com/imaging/java
[8]: https://downloads.aspose.com/imaging/java
[9]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[10]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics
[11]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Font
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.brushes/SolidBrush
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#drawString-java.lang.String-com.aspose.imaging.Font-com.aspose.imaging.Brush-float-float-
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save--
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Font
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.brushes/SolidBrush
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Size
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Matrix
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#setTransform-com.aspose.imaging.Matrix-
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Graphics#drawString-java.lang.String-com.aspose.imaging.Font-com.aspose.imaging.Brush-float-float-
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save--
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/imaging/java/getting-started/
[26]: https://blog.aspose.com/2020/11/20/convert-dicom-to-jpeg-gif-png-bmp-images-in-java/





