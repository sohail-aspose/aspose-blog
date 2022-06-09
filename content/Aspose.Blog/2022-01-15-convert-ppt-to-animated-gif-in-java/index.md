---
title: 'Convert PowerPoint PPT to Animated GIF in Java'
seoTitle: "Convert PowerPoint PPT to GIF in Java | PPT, PPTX to Animated GIF"
description: "Use Java PowerPoint library to convert PPT/PPTX presentations to animated GIF using Java. Customize PPT to GIF conversion dynamically."
date: Sat, 15 Jan 2022 10:12:00 +0000
draft: false
url: /2022/01/15/convert-ppt-to-animated-gif-in-java/
author: Usman Aziz
summary: 'Animated [GIF][1] has the ability to contain a number of images in a single file. Therefore, PowerPoint presentations are often converted to GIF files where each image in the GIF represents a slide. To perform the conversion programmatically, this article covers **how to convert a PowerPoint [PPT][2] or [PPTX][3] presentation to an animated GIF in Java**. Furthermore, you will learn how to customize frame size, the delay between slides, and frames per second programmatically.'
tags: ['Java API for PowerPoint to GIF Conversion', 'powerpoint to gif java', 'ppt to gif java', 'pptx to gif java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PowerPoint-PPT-to-GIF.png" alt="Convert PowerPoint PPT to Animated GIF in Java">}}


Animated [GIF][4] has the ability to contain a number of images in a single file. Therefore, PowerPoint presentations are often converted to GIF files where each image in the GIF represents a slide. To perform the conversion programmatically, this article covers **how to convert a PowerPoint [PPT][5] or [PPTX][6] presentation to an animated GIF in Java**. Furthermore, you will learn how to customize frame size, the delay between slides, and frames per second programmatically.

*   [Java API for PowerPoint to GIF Conversion][7]
*   [Convert a PowerPoint PPT to GIF in Java][8]
*   [Set Additional Options for PPT/PPTX to GIF Conversion][9]

## Java API for PowerPoint PPT to GIF Conversion {#Library-for-PowerPoint-to-GIF-Conversion}

[Aspose.Slides for Java][10] is a feature-rich API for creating and manipulating PowerPoint presentations. Moreover, it provides high-fidelity conversion of PPT/PPTX files to other formats. We will use this API to convert PowerPoint PPT/PPTX files to animated GIFs. You can [download][11] API's JAR or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert a PowerPoint PPT to GIF in Java {#Convert-a-PowerPoint-PPT-to-GIF}

To convert a PPT/PPTX to GIF, you only need to load the presentation and save it as a GIF. The following are the steps to convert a PPT to GIF in Java.

*   Load the PPT/PPTX presentation using [Presentation][12] class.
*   Save the presentation as GIF using [Presentation.save(string, SaveFormat.Gif)][13] method.

The following code sample shows how to convert a PowerPoint PPTX file to an animated GIF in Java.

{{< gist aspose-com-gists 9391d376590f7710bf30223c6ea86423 "ppt-to-gif.java" >}}

## Set Additional Options - Java PPT to GIF {#Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion}

You can also customize PPT to GIF conversion using different options such as the delay between slides, frame size of GIF, and the transition in frames per second. The following are the steps to customize PPT to GIF conversion.

*   Load the PPT/PPTX presentation using [Presentation][14] class.
*   Create an instance of [GifOptions][15] class.
*   Set desired options such as frame size.
*   Save the presentation as GIF using [Presentation.save(string, SaveFormat.Gif, GifOptions)][16] method.

The following code sample shows how to convert a PPT to an animated GIF with customized settings in Java.

{{< gist aspose-com-gists 9391d376590f7710bf30223c6ea86423 "ppt-to-gif-custom.java" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][17] to use Aspose.Slides for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert PowerPoint PPT/PPTX presentations to animated GIF in Java. Furthermore, you have seen how to customize PowerPoint to GIF conversion using different options. Besides, you can explore more about Aspose.Slides for Java using the [documentation][18]. Also, you can post your queries to our [forum][19].

## See Also

*   [Create PowerPoint Presentations using Java][20]
*   [Apply 3D Effects in PowerPoint PPT in Java][21]
*   [Extract Images from PowerPoint PPT in Java][22]
*   [Create and Manipulate Tables in PowerPoint using Java][23]




[1]: https://docs.fileformat.com/image/gif/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: https://docs.fileformat.com/image/gif/
[5]: https://docs.fileformat.com/presentation/ppt/
[6]: https://docs.fileformat.com/presentation/pptx/
[7]: #Library-for-PowerPoint-to-GIF-Conversion
[8]: #Convert-a-PowerPoint-PPT-to-GIF
[9]: #Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion
[10]: https://products.aspose.com/slides/java
[11]: https://downloads.aspose.com/slides/java
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/GifOptions
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/slides/java/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[21]: https://blog.aspose.com/2022/02/04/apply-three-d-effects-in-ppt-in-java/
[22]: https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-java/
[23]: https://blog.aspose.com/2021/09/23/manipulate-tables-in-powerpoint-using-java/




