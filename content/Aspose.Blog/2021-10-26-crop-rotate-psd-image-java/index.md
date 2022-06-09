---
title: 'Crop or Rotate PSD Image in Java'
seoTitle: "Crop or Rotate PSD Image Programmatically in Java"
description: "You can crop or rotate a PSD image file programmatically in Java. Crop any region by shift or crop by rectangle in Java application."
date: Tue, 26 Oct 2021 06:09:00 +0000
draft: false
url: /2021/10/26/crop-rotate-psd-image-java/
author: Farhan Raza
summary: 'PSD image files are used to design pictures for logos, banners, brochures, and many other purposes. In certain scenarios, you may need to crop or rotate a PSD file within your Java applications. This article covers how to crop or rotate a PSD file programmatically using Java.'
tags: ['Crop PSD', 'Crop PSD in Java', 'Resize PSD in Java', 'Rotate PSD', 'Rotate PSD in Java']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/Crop-Resize-PSD.jpg" alt="Crop Resize PSD">}}


[PSD][1] image files are used to design pictures for logos, banners, brochures, and many other purposes. In certain scenarios, you may need to crop or rotate a PSD file within your Java applications. This article covers how to crop or rotate a PSD file programmatically in Java.

*   [Rotate or Crop a PSD File – Java API Installation][2]
*   [Crop PSD Image with Shift Approach in Java][3]
*   [Crop PSD Image with Rectangular Coordinates in Java][4]
*   [Rotate PSD Image at any Angle in Java][5]

## Rotate or Crop a PSD File – Java API Installation {#section1}

[Aspose.PSD for Java][6] API supports working with the PSD and several other Photoshop file formats. You can configure the API by downloading the JAR file from the [New Releases][7], or using the following Maven configurations in your project:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
     <groupId>com.aspose</groupId>
     <artifactId>aspose-psd</artifactId>
     <version>21.7</version>
     <classifier>jdk16</classifier>
</dependency>
```

## Crop PSD Image with Shift Approach in Java {#section2}

You can crop a PSD image by shifting the contents as per your requirements. Please follow the steps below for cropping the image by shifting contents:

1.  Load the input PSD file into a [RasterImage][8] class object.
2.  Cache the image using [cacheData][9] method.
3.  Define shift values and pass them to the [crop][10] method.
4.  Save output cropped image.

The following code shows how to crop a PSD image by shifting content programmatically in Java:

{{< gist aspose-com-gists f5a0ac6f93bd0aec0c737546f8b900de "Crop-PSD-Image-Shift.java" >}}

## Crop PSD Image with Rectangular Coordinates in Java {#section3}

You can crop any rectangular region in a PSD image by specifying the coordinates. You need to follow the below steps to crop a PSD image:

1.  Load an existing image into an instance of [RasterImage][11] class.
2.  Cache the image for better performance.
3.  Create an instance of [Rectangle][12] class with the desired size.
4.  Crop the image using the [crop][13] method and save output file.

The code snippet below demonstrates how to crop a PSD file with rectangular coordinates in Java:

{{< gist aspose-com-gists f5a0ac6f93bd0aec0c737546f8b900de "Crop-PSD-Image-Rectangle.java" >}}

## Rotate PSD Image at any Angle in Java {#section4}

In some situations, you might need to rotate the PSD images at a specific angle. Please follow the steps below for rotating a PSD image:

1.  Load the source PSD image file with [RasterImage][14] class.
2.  Before rotation, the image should be cached for improved performance.
3.  Specify the angle for rotation in the [rotate][15] method.
4.  Save the output file.

The below code sample explains how to rotate a PSD image in Java:

{{< gist aspose-com-gists f5a0ac6f93bd0aec0c737546f8b900de "Rotate-PSD-Angle.java" >}}

## Get Free Evaluation License

You may request a [free temporary license][16] to evaluate the API without any limitations.

## Conclusion

In this article, you have learned different approaches to crop a PSD image or rotate it at a specific angle. The API offers several other features to work with PSD and other supported file formats. Moreover, please take a look at the API [Documentation][17] for more information. Feel free to contact us at the [Free Support Forum][18] for any of your inquiries.

## See Also

[Convert PSD to TIFF Image Programmatically with Java][19]




[1]: https://docs.fileformat.com/image/psd/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/psd/java
[7]: https://downloads.aspose.com/psd/java
[8]: https://apireference.aspose.com/psd/java/com.aspose.psd.class-use/RasterImage
[9]: https://apireference.aspose.com/psd/java/com.aspose.psd/DataStreamSupporter#cacheData--
[10]: https://apireference.aspose.com/psd/java/com.aspose.psd/RasterImage#crop-int-int-int-int-
[11]: https://apireference.aspose.com/psd/java/com.aspose.psd.class-use/RasterImage
[12]: https://apireference.aspose.com/psd/java/com.aspose.psd/rectangle
[13]: https://apireference.aspose.com/psd/java/com.aspose.psd/RasterImage#crop-com.aspose.psd.Rectangle-
[14]: https://apireference.aspose.com/psd/java/com.aspose.psd.class-use/RasterImage
[15]: https://apireference.aspose.com/psd/java/com.aspose.psd/RasterImage#rotate-float-
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/psd/java/
[18]: https://forum.aspose.com/c/psd
[19]: https://blog.aspose.com/2021/10/01/convert-psd-tiff-java/




