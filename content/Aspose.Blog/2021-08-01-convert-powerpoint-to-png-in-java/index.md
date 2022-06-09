---
title: 'Convert PowerPoint PPTX/PPT to PNG Images in Java'
seoTitle: "PowerPoint to PNG in Java | PPTX to PNG, PPT to PNG | Java API"
description: "Use Java PowerPoint API to convert PowerPoint presentations to PNG images using Java. Convert PPTX to PNG and PPT to PNG using Java."
date: Sun, 01 Aug 2021 15:59:00 +0000
draft: false
url: /2021/08/01/convert-powerpoint-to-png-in-java/
author: Usman Aziz
summary: 'The conversion of PowerPoint presentations to image formats could be used in various scenarios. For example, to display the presentations in your web or desktop applications, to generate thumbnails, etc. Since [PNG][1] is one of the most popular image formats, in this article, you will learn **how to convert slides in PowerPoint PPTX or PPT to PNG images using Java**.'
tags: ['PPT to PNG Java', 'PPTX to PNG Java', 'PowerPoint to PNG Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-PNG-Image.jpg" alt="">}}


The conversion of PowerPoint presentations to image formats could be used in various scenarios. For example, to display the presentations in your web or desktop applications, to generate thumbnails, etc. Since [PNG][2] is one of the most popular image formats, in this article, you will learn **how to convert slides in PowerPoint PPTX or PPT to PNG images using Java**.

*   [API for PowerPoint to PNG Conversion][3]
*   [Convert PowerPoint PPTX or PPT to PNG][4]

## Java API for PowerPoint to PNG Conversion {#API-for-PowerPoint-to-PNG-Conversion}

For PPTX or PPT to PNG conversion, we will use [Aspose.Slides for Java][5]. The API lets you create, manipulate and convert PowerPoint and OpenOffice presentations from within the Java applications. You can either [download][6] the API or install it using the following Maven configurations.

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
    <artifactId>aspose-slides</artifactId>
    <version>21.8</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert PowerPoint PPTX or PPT to PNG in Java {#Convert-PowerPoint-PPTX-or-PPT-to-PNG}

The following are the steps to convert slides in a PowerPoint PPTX to PNG images using Java.

1.  First, create an instance of the [Presentation][7] class to load the presentation.
2.  Define the dimensions of the resultant PNG image.
3.  Loop through each [ISlide][8] in [Presentation.getSlides()][9] collection.
4.  Generate image of the each slide using [ISlide.getThumbnail(float ScaleX, float ScaleY)][10] method and get the reference of image into a [BufferedImage][11] object.
5.  Create a new File for the output PNG image.
6.  Finally, save the PNG image using [ImageIO.write(BufferedImage, String, File)][12] method.

The following code sample shows how to convert a PowerPoint PPTX to PNG.

{{< gist aspose-com-gists a81ec561782f677a7ee6c4f540ffd411 "powerpoint-to-png.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][13].

## Online Demo

Try the [online PowerPoint to PNG converter][14], which is based on Aspose.Slides.

## Conclusion

In this article, you have learned how to convert slides in PowerPoint PPTX or PPT to PNG using Java. You can simply install the API and use the provided code in your Java applications. In addition, you can visit the [documentation][15] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][16].

## See Also

*   [Create MS PowerPoint Presentations in Java][17]




[1]: https://docs.fileformat.com/image/png/
[2]: https://docs.fileformat.com/image/png/
[3]: #API-for-PowerPoint-to-PNG-Conversion
[4]: #Convert-PowerPoint-PPTX-or-PPT-to-PNG
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getThumbnail-float-float-
[11]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[12]: https://docs.oracle.com/javase/7/docs/api/javax/imageio/ImageIO.html#write(java.awt.image.RenderedImage,%20java.lang.String,%20java.io.File)
[13]: https://purchase.aspose.com/temporary-license
[14]: https://products.aspose.app/slides/conversion/pptx-to-png
[15]: https://docs.aspose.com/slides/java
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





