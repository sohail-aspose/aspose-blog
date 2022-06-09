---
title: 'Convert PowerPoint PPTX/PPT to TIFF using Java'
seoTitle: "Convert PowerPoint PPTX/PPT to TIFF using Java | Custom Size or Pixel"
description: "Use Java PowerPoint API to convert PowerPoint PPTX or PPT to TIFF using Java. Customize the image size and pixel format in PPTX/PPT to TIFF conversion."
date: Tue, 13 Jul 2021 17:33:00 +0000
draft: false
url: /2021/07/13/convert-powerpoint-to-tiff-using-java/
author: Usman Aziz
summary: 'In various scenarios, such as printing, fax, etc., PowerPoint to [TIFF][1] conversion is used. To automate this conversion from within a web or desktop application, this article covers **how to convert PowerPoint PPTX/PPT to TIFF using Java**. Furthermore, it also shows how to customize the size and pixel format of the resultant TIFF images.'
tags: ['Java PowerPoint to TIFF Converter', 'ppt to tiff java', 'pptx to tiff java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-TIFF.jpg" alt="PowerPoint to TIFF Java">}}


In various scenarios, such as printing, fax, etc., PowerPoint to [TIFF][2] conversion is used. To automate this conversion from within a web or desktop application, this article covers **how to convert PowerPoint PPTX/PPT presentations to TIFF using Java**. Furthermore, it also shows how to customize the size and pixel format of the resultant TIFF images.

*   [Java PowerPoint to TIFF Converter][3]
*   [Convert PowerPoint to TIFF][4]
*   [Convert PowerPoint to TIFF with Custom Image Size][5]
*   [PPTX to TIFF with Custom Pixel Format][6]

**TIP:** You may want to check out **Aspose FREE online [PowerPoint to Poster Converter][7].**

## Java PowerPoint to TIFF Converter {#PowerPoint-to-TIFF-Converter}

In order to convert the presentations to TIFF images, we will use [Aspose.Slides for Java][8]. The said API lets you create, manipulate and convert presentation documents from within the Java applications. You can either [download][9] the API or install it using the following Maven configurations.

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
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert PowerPoint PPTX to TIFF using Java {#Convert-PowerPoint-to-TIFF}

The following are the steps to convert a PowerPoint PPTX/PPT to TIFF using Java.

*   First, load the PowerPoint presentation using [Presentation][10] class.
*   Then, convert PPTX to TIFF using [Presentation.save(String, SaveFormat.Tiff)][11] method.

The following code sample shows how to convert a PowerPoint PPTX to TIFF.

{{< gist aspose-com-gists 76149d701f6dfaf85bdce4b5b0dcf09d "powerpoint-to-tiff.java" >}}

## Java Convert PowerPoint to TIFF with Custom Image Size {#Convert-PowerPoint-to-TIFF-with-Custom-Image-Size}

Aspose.Slides for Java also allows you to customize the size of the resultant image in PowerPoint to TIFF conversion. The following are the steps to achieve this.

*   First, load the PowerPoint presentation using [Presentation][12] class.
*   Create an instance of [TiffOptions][13] class.
*   Set image size using [TiffOptions.setImageSize()][14] method.
*   Finally, convert PPTX to TIFF using [Presentation.save(String, SaveFormat.Tiff)][15] method.

The following code sample shows how to convert PPTX to TIFF with custom image size.

{{< gist aspose-com-gists 76149d701f6dfaf85bdce4b5b0dcf09d "powerpoint-to-tiff-image-size.java" >}}

## Convert PowerPoint to TIFF with Custom Pixel Format {#PPTX-to-TIFF-with-Custom-Pixel-Format}

The following are the steps to customize the pixel format in PPTX to TIFF conversion using Java.

*   First, load the PowerPoint presentation using [Presentation][16] class.
*   Create an instance of [TiffOptions][17] class.
*   Set pixel format to desired format using [TiffOptions.setPixelFormat()][18] method.
*   Finally, convert PPTX to TIFF using [Presentation.save(String, SaveFormat.Tiff)][19] method.

The following code sample shows how to customize pixel format in PPTX to TIFF conversion.

{{< gist aspose-com-gists 76149d701f6dfaf85bdce4b5b0dcf09d "powerpoint-to-tiff-pixel-format.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][20].

## Conclusion

In this article, you have seen how to convert PowerPoint PPTX/PPT to TIFF using Java. Furthermore, the step-by-step guide and code samples have shown how to customize the size and pixel format of the resultant TIFF images. You can visit the [documentation][21] to explore other features of Aspose.Slides for Java. In addition, you can feel free to let us know about your queries via our [forum][22].

## See Also

*   [Create PowerPoint Presentations in Java][23]




[1]: https://docs.fileformat.com/image/tiff/
[2]: https://docs.fileformat.com/image/tiff/
[3]: #PowerPoint-to-TIFF-Converter
[4]: #Convert-PowerPoint-to-TIFF
[5]: #Convert-PowerPoint-to-TIFF-with-Custom-Image-Size
[6]: #PPTX-to-TIFF-with-Custom-Pixel-Format
[7]: https://products.aspose.app/slides/conversion/convert-ppt-to-poster-online
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/TiffOptions
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/TiffOptions#setImageSize-java.awt.Dimension-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/TiffOptions
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/TiffOptions#setPixelFormat-int-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/slides/java/developer-guide/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





