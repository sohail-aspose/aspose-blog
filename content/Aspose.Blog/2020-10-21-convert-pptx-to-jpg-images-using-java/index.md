---
title: 'Convert PowerPoint PPTX to JPG Images using Java'
seoTitle: "PPTX to JPG using Java | Convert PPTX Slides to JPG Images in Java"
description: "Convert PowerPoint PPTX to JPG images using Java. Generate thumbnails by converting slides in PPTX to JPG images from within your Java applications."
date: Wed, 21 Oct 2020 23:02:00 +0000
draft: false
url: /2020/10/21/convert-pptx-to-jpg-images-using-java/
author: Usman Aziz
summary: ''
tags: ['convert pptx to jpg in java', 'java pptx to jpg conversion', 'pptx to jpg java converter']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-Image-in-C.png" alt="PPTX to JPG Java">}}


MS PowerPoint presentations can not be displayed directly from within the web or desktop applications. One of the possible solutions is converting the slides in a [PPTX][1] presentation to the images such as [JPEG][2] or [PNG][3]. In accordance with the above-mentioned scenario, this article will show you **how to convert slides in a PPTX to JPG images using Java**.

*   [PPTX to JPG Conversion API][4]
*   [Convert PPTX to JPG Image using Java][5]
*   [Customize Image Dimensions in PPTX to JPG Conversion][6]

**TIP:**

To see a implementation of the conversion process described here, you may want to check out Aspose online [PPT to JPG][7] converter.

## Java PPTX to JPG Image Conversion API {#Java-PPTX-to-JPG-Image-Conversion-API}

[Aspose.Slides for Java][8] is a presentation manipulation API that lets you implement PowerPoint automation features from within your Java applications. In addition, it also provides a PPTX to JPG image converter API to generate thumbnails of the slides in a presentation. You can either [download][9] the API or get it installed using the Maven configuration.

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
    <classifier>jdk16</classifier>
</dependency>
```

## PPTX to JPG Java Conversion

In order to convert the PPTX slides to JPG, you can simply loop through the slides in a presentation and save each of them as a JPG file. The following are the steps to perform this operation.

*   Load the PowerPoint PPTX file using the [Presentation][10] class.
*   Retrieve the slides in presentation using [Presentation.getSlides()][11] method.
*   Access each slide using the [ISlide][12] interface.
*   Get slide's thumbnail into a [BufferedImage][13] object using [ISlide.getThumbnail(1f, 1f)][14] method.
*   Save the _BufferedImage_ as a JPG file.

The following code sample shows how to convert PPTX slide to JPG image using Java.

{{< gist aspose-com-gists ec402be9a402ba91e80a585235f24743 "pptx-to-jpg.java" >}}

### PowerPoint PPTX



{{< figure align=center src="images/Presentation.png" alt="PowerPoint PPTX ">}}


### Converted JPG Images



{{< figure align=center src="images/PPT-to-JPG-in-C.png" alt="Java PPTX to JPG Conversion">}}


## Java PPTX to JPG - Customize Image Dimensions {#Customized-Image-Dimensions-in-PPTX-to-JPG-in-Java}

You can also customize the dimensions to scale the converted JPG images as per your desires. The following are the steps to specify the Scale X and Scale Y values in PPTX to JPG conversion.

*   Load the PowerPoint PPTX file using the [Presentation][15] class.
*   Specify the scaling values for the x-axis and y-axis using the slide's width and height respectively.
*   Retrieve the slides in presentation using [Presentation.getSlides()][16] method.
*   Access each slide using the [ISlide][17] interface.
*   Get slide's thumbnail into a [BufferedImage][18] object using [ISlide.getThumbnail(ScaleX, ScaleY)][19] method.
*   Save the _BufferedImage_ as a JPG file.

The following code sample shows how to apply customized scaling in PPTX to JPG conversion.

{{< gist aspose-com-gists ec402be9a402ba91e80a585235f24743 "pptx-to-jpg-customized.java" >}}

## Conclusion

In this article, you have learned how to convert slides in PPTX to JPG images using Java. Furthermore, you have seen how to apply the desired scaling to the images in PPTX to JPG conversion. You can learn more about the Java presentation manipulation API using [documentation][20].

## See Also

*   [Convert PowerPoint PPTX to PDF using Java][21]




[1]: https://docs.fileformat.com/presentation/pptx/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: #Java-PPTX-to-JPG-Image-Conversion-API
[5]: #Convert-PPTX-to-JPG-Image-using-Java
[6]: #Customized-Image-Dimensions-in-PPTX-to-JPG-in-Java
[7]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[13]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getThumbnail-float-float-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[18]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getThumbnail-float-float-
[20]: https://docs.aspose.com/slides/java
[21]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/





