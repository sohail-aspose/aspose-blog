---
title: 'Adjust Image Contrast, Brightness, and Gamma in Java'
seoTitle: "Java: Adjust Image Contrast, Brightness, Gamma | Java Image Editor"
description: "Use Java image processing API to adjust contrast, brightness, and gamma of images in java. Implement image editing features in your Java applications."
date: Sat, 27 Nov 2021 14:59:00 +0000
draft: false
url: /2021/11/27/adjust-image-contrast-brightness-gamma-in-java/
author: Usman Aziz
summary: 'Various characteristics of images are modified to enhance their appearance. [Contrast][1], [brightness][2], and [gamma][3] are among the most commonly used attributes to improve the quality of the images. In various cases, you have to control these attributes programmatically from within your Java applications. To achieve that, in this article, you will learn **how to adjust the contrast, brightness, and gamma of an image in Java**.'
tags: ['Adjust Brightness of an Image in Java', 'Adjust Contrast of an Image in Java', 'Java Image Editing API', 'Modify Gamma of an Image in Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Adjust-Image-Contrast-Brightness-Gamma-Java-2.png" alt="Adjust Image Contrast, Brightness, and Gamma in Java">}}


Various characteristics of images are modified to enhance their appearance. [Contrast][4], [brightness][5], and [gamma][6] are among the most commonly used attributes to improve the quality of the images. In various cases, you have to control these attributes programmatically from within your Java applications. To achieve that, in this article, you will learn **how to adjust the contrast, brightness, and gamma of an image in Java**.

*   [Java Image Editing API][7]
*   [Adjust Contrast of an Image in Java][8]
*   [Adjust Brightness of an Image in Java][9]
*   [Modify Gamma of an Image in Java][10]

## Java API to Adjust Image Contrast, Brightness, and Gamma {#Image-Editing-API}

To control the contrast, brightness, and gamma of images, we will use [Aspose.Imaging for Java][11]. It is a powerful image processing API that supports a [wide range of image formats][12]. Using the API, you can edit images seamlessly without writing complex code. You can [download][13] the API's JAR and add its reference to your project. Also, you can install it into your Maven-based applications by adding the following configurations in **pom.xml**.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-imaging-java</artifactId>
    <version>21.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Adjust Contrast of an Image in Java {#Adjust-Contrast-of-an-Image}

The difference in pixel intensity of an image is known as contrast. The contrast value is increased or decreased to control the visibility of objects in an image. Increasing the contrast at a certain level makes the image look more clear. Whereas, decreasing the contrast value makes the objects less distinguishable.

The following are the steps to adjust the contrast of an image in Java.

*   First, use [RasterImage][14] class to load the image.
*   Then, use [RasterImage.cacheData()][15] method to cache image if it isn't already.
*   Use [RasterImage.adjustContrast(float)][16] method to set contrast value in range \[-100, 100\].
*   Finally, save the image using [RasterImage.save(string)][17] method.

The following code sample shows how to adjust the contrast of an image in Java.

{{< gist aspose-com-gists 99f3272cfbe5139edcb43f7d7bfacb3e "adjust-image-contrast.java" >}}

The following is the comparison of input and output images after increasing the contrast value.



{{< figure align=center src="images/Adjust-Image-Contrast.png" alt="Adjust Contrast of Images in Java" caption="Adjust Image Contrast">}}


## Adjust Brightness of an Image in Java {#Adjust-Brightness-of-an-Image}

The brightness is adjusted to increase or decrease the darkness or lightness of an image. Let's have a look at how to modify the brightness of an image in Java.

*   First, use [RasterImage][18] class to load the image.
*   Then, use [RasterImage.cacheData()][19] method to cache image if it isn't already.
*   Adjust brightness of the image using [RasterImage.adjustBrightness(int)][20] method.
*   Finally, save the image using [RasterImage.save(string)][21] method.

The following code sample shows how to adjust the brightness of an image in Java.

{{< gist aspose-com-gists 99f3272cfbe5139edcb43f7d7bfacb3e "adjust-image-brightness.java" >}}

The following is the comparison of input and output images after modifying brightness.



{{< figure align=center src="images/Adjust-Image-Brightness.png" alt="Adjust Brightness of Images in Java" caption="Adjust Image Brightness">}}


## Adjust Gamma of an Image in Java {#Modify-Gamma-of-an-Image}

The gamma attribute controls the ratio of red, green, and blue colors in an image. Also, it affects the brightness of the image. The following are the steps to adjust the gamma of an image in Java.

*   First, use [RasterImage][22] class to load the image.
*   Then, use [RasterImage.cacheData()][23] method to cache image if it isn't already.
*   To change gamma of the image, use [RasterImage.adjustGamma(float, float, float)][24] method.
*   Finally, save the image using [RasterImage.save(string)][25] method.

The following code sample shows how to adjust the gamma of an image in Java.

{{< gist aspose-com-gists 99f3272cfbe5139edcb43f7d7bfacb3e "adjust-image-gamma.java" >}}

The following is the comparison of input and output images after modifying the gamma value.



{{< figure align=center src="images/Adjust-Image-Gamma.png" alt="Adjust Gamma of Images in Java" caption="Adjust Image Gamma">}}


## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][26] to use Aspose.Imaging for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to adjust the contrast, brightness, and gamma of images in Java. Furthermore, the code samples have demonstrated how modifying the values of contrast, brightness, and gamma affects an image. To explore more about Java image processing API, visit [documentation][27]. Also, you can download the source code samples of the API from [GitHub][28]. In case of any queries, contact us at our [forum][29].

## See Also

*   [Resize Images in Java][30]
*   [Rotate or Flip Images in Java][31]
*   [Add Watermark to Images using Java][32]
*   [Compress Images in Java][33]




[1]: https://en.wikipedia.org/wiki/Contrast_(vision)
[2]: https://en.wikipedia.org/wiki/Brightness
[3]: https://en.wikipedia.org/wiki/Gamma_correction
[4]: https://en.wikipedia.org/wiki/Contrast_(vision)
[5]: https://en.wikipedia.org/wiki/Brightness
[6]: https://en.wikipedia.org/wiki/Gamma_correction
[7]: #Image-Editing-API
[8]: #Adjust-Contrast-of-an-Image
[9]: #Adjust-Brightness-of-an-Image
[10]: #Modify-Gamma-of-an-Image
[11]: https://products.aspose.com/imaging/java/
[12]: https://docs.aspose.com/imaging/java/supported-file-formats/
[13]: https://downloads.aspose.com/imaging/java/
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#cacheData--
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#adjustContrast-float-
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#cacheData--
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#adjustBrightness-int-
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/DataStreamSupporter#cacheData--
[24]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/RasterImage#adjustGamma-float-float-float-
[25]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/imaging/java/
[28]: https://github.com/aspose-imaging/Aspose.Imaging-for-Java
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2021/11/22/resize-images-in-java/
[31]: https://blog.aspose.com/2021/11/21/rotate-and-flip-images-in-java/
[32]: https://blog.aspose.com/2021/01/27/add-watermark-to-images-using-java/
[33]: https://blog.aspose.com/2021/02/26/compress-png-jpeg-tiff-images-in-java/




