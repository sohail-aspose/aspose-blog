---
title: 'Rotate and Flip Images in Java'
seoTitle: "Rotate and Flip Images in Java | Java Image Editor Library"
description: "Use Java image processing API to rotate and flip images using Java. Rotate image only, flip image only, or rotate and flip image at the same time."
date: Sun, 21 Nov 2021 14:11:00 +0000
draft: false
url: /2021/11/21/rotate-and-flip-images-in-java/
author: Usman Aziz
summary: 'Image rotation and flipping are among the key features of the image editors. While working with images or creating your own image editor in Java, you may need to implement these features. To achieve that, this article shows **how to rotate and flip images programmatically in Java**. Particularly, we will cover how to rotate an image, flip an image, and rotate and flip an image at the same time.'
tags: ['Flip an Image in Java', 'Java API to Rotate and Flip Images', 'Java Image Editor Library', 'Rotate an Image in Java', 'Rotate an Image on a Particular Angle in Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Rotate-Flip-Images-Logo.jpg" alt="Rotate or Flip images in Java">}}


Image rotation and flipping are among the key features of the image editors. While working with images or creating your own image editor in Java, you may need to implement these features. To achieve that, this article shows **how to rotate and flip images programmatically in Java**. Particularly, we will cover how to rotate an image, flip an image, and rotate and flip an image at the same time.

*   [Java API to Rotate and Flip Images][1]
*   [Rotate and Flip an Image][2]
    *   [Rotate an Image in Java][3]
    *   [Flip an Image in Java][4]
    *   [Rotate and Flip an Image in Java][5]
*   [Rotate an Image on a Particular Angle][6]

## Java API to Rotate and Flip Images {#API-to-Rotate-and-Flip-Images}

[Aspose.Imaging for Java][7] is an image processing API that allows you to manipulate a wide range of image formats. The API makes it quite easier for you to manipulate images without writing a lot of code. You can [download][8] the API or install it into your Java applications using the following Maven configurations.

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

## Rotate and Flip an Image in Java {#Rotate-and-Flip-an-Image}

You can either rotate an image at a particular angle or the standard rotation angles which are 90, 180, and 270 degrees. In addition, the image can be flipped horizontally or vertically. Aspose.Imaging for Java provides a single method to rotate as well as flip an image. The [RotateFlipType][9] enum is used to specify the rotation angle and flip type. You can perform one of the following operations on an image:

*   Rotate an image
*   Flip an image
*   Rotate and flip an image at the same time

### Rotate an Image in Java {#Rotate-an-Image}

To rotate an image without flipping, you can choose one of the following values of **RotateFlipType** enum.

*   **Rotate180FlipNone**: 180-degree rotation without flipping
*   **Rotate270FlipNone**: 270-degree rotation without flipping
*   **Rotate90FlipNone**: 90-degree rotation without flipping

Let's see how to rotate an image at 270 degrees in Java.

*   First, use [Image][10] class to load the image.
*   Then, use [Image.rotateFlip(RotateFlipType.Rotate270FlipNone)][11] method to rotate image to 270 degrees.
*   Finally, save resultant image using [Image.save(string)][12] method.

The following code snippet shows how to rotate an image in Java.

{{< gist aspose-com-gists f9675e00226911e7351c3e80fc4c2baf "rotate-image.java" >}}

The following are the input image (left) and the resultant image (right) that we get after rotation.



{{< figure align=center src="images/Rotate-Image.png" alt="rotate an image in java" caption="Rotate an Image">}}


### Flip an Image in Java {#Flip-an-Image}

To flip an image, the following **RotateFlipType** values are used.

*   **RotateNoneFlipX**: No rotation with horizontal flipping
*   **RotateNoneFlipY**: No rotation with vertical flipping
*   **RotateNoneFlipXY**: No rotation with horizontal and vertical flipping

The following are the steps to flip an image in Java.

*   First, load the image using [Image][13] class.
*   Then, use [Image.rotateFlip(RotateFlipType.RotateNoneFlipX)][14] method to flip the image horizontally.
*   Finally, save resultant image using [Image.save(string)][15] method.

The following code sample shows how to flip an image.

{{< gist aspose-com-gists f9675e00226911e7351c3e80fc4c2baf "flip-image.java" >}}

The following are the input image and the resultant flipped image.



{{< figure align=center src="images/Flip-Image.png" alt="Flip an image in Java" caption="Flip an Image">}}


### Rotate and Flip an Image in Java {#Rotate-and-Flip-an-Image-at-once}

In the previous sections, you have seen how to either rotate an image or flip it. However, in some cases, you have to perform both operations at the same time. To achieve this, the following **RotateFlipType** values are used.

*   **Rotate180FlipX**: 180-degree rotation with horizontal flipping
*   **Rotate180FlipXY**: 180-degree rotation with horizontal and vertical flipping
*   **Rotate180FlipY**: 180-degree rotation with vertical flipping
*   **Rotate270FlipX**: 270-degree rotation with horizontal flipping
*   **Rotate270FlipXY**: 270-degree rotation with horizontal and vertical flipping
*   **Rotate270FlipY**: 270-degree rotation with vertical flipping
*   **Rotate90FlipX**: 90-degree rotation with horizontal flipping
*   **Rotate90FlipXY**: 90-degree rotation with horizontal and vertical flipping
*   **Rotate90FlipY**: 90-degree rotation with vertical flipping

The following are the steps to rotate and flip an image at the same time in Java.

*   First, use [Image][16] class to load an image.
*   Then, use [Image.rotateFlip(RotateFlipType.Rotate180FlipX)][17] method to rotate and flip the image.
*   Finally, save resultant image using [Image.save(string)][18] method.

The following code snippet shows how to perform rotation and flipping of an image at the same time.

{{< gist aspose-com-gists f9675e00226911e7351c3e80fc4c2baf "rotate-flip-image.java" >}}

The following is the resultant image (right) that we get after applying rotation and flipping.



{{< figure align=center src="images/Rotate-and-Flip-Image.png" alt="Rotate and flip an image in Java" caption="Rotate and Flip an Image">}}


## Rotate Image on a Particular Angle {#Rotate-an-Image-on-a-Particular-Angle}

You can also rotate an image at an angle other than 90, 180, and 270. For this, the API provides the [Image.rotate(float angle)][19] method which accepts the rotation angle as a parameter. The following code sample shows how to rotate an image at 20 degrees in Java.

{{< gist aspose-com-gists f9675e00226911e7351c3e80fc4c2baf "rotate-image-on-angle.java" >}}

The following is the output of the code sample above.



{{< figure align=center src="images/rotate-image-1.png" alt="rotate image at particular angle in java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][20] to use Aspose.Imaging for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to rotate and flip images in Java. Furthermore, you have seen how to rotate an image, flip an image, and rotate and flip an image at the same time. In addition, the article also covered how to rotate an image at a particular angle other than 90, 180, and 270 degrees. In case you want to explore more about the Java image processing API, visit [documentation][21]. Also, you can download the source code samples of the API from [GitHub][22]. In case of any questions, you can reach us at our [forum][23].

## See Also

*   [Resize Images in Java][24]
*   [Compress Images in Java][25]
*   [Add Watermark to Images using Java][26]




[1]: #API-to-Rotate-and-Flip-Images
[2]: #Rotate-and-Flip-an-Image
[3]: #Rotate-an-Image
[4]: #Flip-an-Image
[5]: #Rotate-and-Flip-an-Image-at-once
[6]: #Rotate-an-Image-on-a-Particular-Angle
[7]: https://products.aspose.com/imaging/java/
[8]: https://downloads.aspose.com/imaging/java/
[9]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RotateFlipType
[10]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[11]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#rotateFlip-int-
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#rotateFlip-int-
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#rotateFlip-int-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#rotate-float-
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/imaging/java/
[22]: https://github.com/aspose-imaging/Aspose.Imaging-for-Java
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/11/22/resize-images-in-java/
[25]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/
[26]: https://blog.aspose.com/2021/01/27/add-watermark-to-images-using-java/




