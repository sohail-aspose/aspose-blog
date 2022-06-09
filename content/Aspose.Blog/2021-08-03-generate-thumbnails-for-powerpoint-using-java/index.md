---
title: 'Generate Thumbnails for PowerPoint PPTX or PPT using Java'
seoTitle: "Generate Thumbnails of PPTX PPT in Java | Aspose PowerPoint API"
description: "Use Java PowerPoint API to generate thumbnails of PPTX or PPT presentations using Java. Generate thumbnails with desired dimensions."
date: Tue, 03 Aug 2021 18:14:00 +0000
draft: false
url: /2021/08/03/generate-thumbnails-for-powerpoint-using-java/
author: Usman Aziz
summary: '[Thumbnails][1] are small-sized versions of the larger images that make it easier to look at or scroll through the list of images. MS PowerPoint also uses thumbnails for the presentations to go through the content and navigate to a particular slide. In this article, you will learn **how to generate thumbnails of PowerPoint PPTX or PPT using Java**. You can use this feature in scenarios such as while creating your web or desktop-based PowerPoint viewer.'
tags: ['Generate Thumbnails for PPT in Java', 'Generate Thumbnails for PPTX in Java', 'Generate Thumbnails for PowerPoint in Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Generate-PPTX-Thumbnails.jpg" alt="Generate PPTX thumbnails in Java">}}


[Thumbnails][2] are small-sized versions of the larger images that make it easier to look at or scroll through the list of images. MS PowerPoint also uses thumbnails for the presentations to go through the content and navigate to a particular slide. In this article, you will learn **how to generate thumbnails of PowerPoint PPTX or PPT using Java**. You can use this feature in scenarios such as while creating your web or desktop-based PowerPoint viewer.

*   [Java API to Generate Thumbnails for PowerPoint PPTX/PPT][3]
*   [Generate Thumbnails for PowerPoint PPTX/PPT][4]
*   [Generate Thumbnails with User-Defined Dimensions][5]

## Java API to Generate Thumbnails for PowerPoint PPTX/PPT {#API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT}

To generate thumbnails for PPTX or PPT presentations, we will use [Aspose.Slides for Java][6]. It is a feature-rich API for creating, manipulating, and converting PowerPoint and OpenOffice presentations. You can either [download][7] the API or install it using the following Maven configurations.

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

## Generate Thumbnails for PPTX or PPT using Java {#Generate-Thumbnails-for-PPTX-PPT}

The following are the steps to generate thumbnails of a PPTX presentation using Java.

1.  First, create an instance of the [Presentation][8] class to load the presentation.
2.  Loop through each [ISlide][9] in [Presentation.getSlides()][10] collection.
3.  Generate image of the each slide using [ISlide.getThumbnail(1f, 1f)][11] method and get the reference of image into a [BufferedImage][12] object.
4.  Create a new [File][13] for the output image.
5.  Finally, save the image using [ImageIO.write(BufferedImage, String, File)][14] method.

The following code sample shows how to generate thumbnails of a PPTX presentation using Java.

{{< gist aspose-com-gists 9f9c8614b881fa83354e701d1a923a2a "generate-pptx-thumbnail.java" >}}

## Generate Thumbnails with User-Defined Dimensions {#Generate-Thumbnails-with-User-Defined-Dimensions}

You can also specify your own dimensions for the thumbnail images using the height and width of the slides. The following are the steps to perform this operation.

1.  First, create an instance of the [Presentation][15] class to load the presentation.
2.  Define the dimensions of the resultant PNG image.
3.  Loop through each [ISlide][16] in [Presentation.getSlides()][17] collection.
4.  Generate image of the each slide using [ISlide.getThumbnail(float ScaleX, float ScaleY)][18] method and get the reference of image into a [BufferedImage][19] object.
5.  Create a new [File][20] for the output image.
6.  Finally, save the image using [ImageIO.write(BufferedImage, String, File)][21] method.

The following code sample shows how to generate thumbnails of a PPTX with customized dimensions.

{{< gist aspose-com-gists 9f9c8614b881fa83354e701d1a923a2a "generate-pptx-thumbnail-custom-dimension.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][22].

## Conclusion

In this article, you have learned how to generate thumbnails of PowerPoint PPTX or PPT using Java. Moreover, you have seen how to generate thumbnails with user-defined dimensions. In addition, you can visit the [documentation][23] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][24].

## See Also

*   [Create MS PowerPoint Presentations in Java][25]
*   [Add Watermark to PowerPoint Slides using Java][26]
*   [Extract Text from PowerPoint Files using Java][27]




[1]: https://en.wikipedia.org/wiki/Thumbnail
[2]: https://en.wikipedia.org/wiki/Thumbnail
[3]: #API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT
[4]: #Generate-Thumbnails-for-PPTX-PPT
[5]: #Generate-Thumbnails-with-User-Defined-Dimensions
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java/
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getThumbnail-float-float-
[12]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[13]: https://docs.oracle.com/javase/7/docs/api/java/io/File.html
[14]: https://docs.oracle.com/javase/7/docs/api/javax/imageio/ImageIO.html#write(java.awt.image.RenderedImage,%20java.lang.String,%20java.io.File)
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getThumbnail-float-float-
[19]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[20]: https://docs.oracle.com/javase/7/docs/api/java/io/File.html
[21]: https://docs.oracle.com/javase/7/docs/api/javax/imageio/ImageIO.html#write(java.awt.image.RenderedImage,%20java.lang.String,%20java.io.File)
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/slides/java
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[26]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[27]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/





