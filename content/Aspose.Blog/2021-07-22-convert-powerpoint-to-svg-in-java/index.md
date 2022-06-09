---
title: 'Convert PowerPoint Presentations to SVG in Java'
seoTitle: "Convert PowerPoint to SVG in Java | PPTX to SVG | PPT to SVG"
description: "Use Java PowerPoint API to convert PowerPoint PPTX/PPT to SVG using Java. Create your own PowerPoint viewer Java Spring or other Java applications."
date: Thu, 22 Jul 2021 16:21:00 +0000
draft: false
url: /2021/07/22/convert-powerpoint-to-svg-in-java/
author: Usman Aziz
summary: 'PowerPoint to [SVG][1] conversion is often performed to display the presentations in web or desktop applications. Various PowerPoint viewers also convert the presentations to SVG for slideshow. Accordingly, this article covers **how to convert PowerPoint PPTX or PPT presentations to SVG files using Java**.'
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-SVG.jpg" alt="PowerPoint to SVG Java">}}


PowerPoint to [SVG][2] conversion is often performed to display the presentations in web or desktop applications. Various PowerPoint viewers also convert the presentations to SVG for slideshow. Accordingly, this article covers **how to convert PowerPoint PPTX or PPT presentations to SVG files using Java**.

*   [PowerPoint to SVG Converter][3]
*   [Convert PPTX/PPT to SVG in Java][4]

## Java PowerPoint to SVG Converter {#PowerPoint-Presentation-to-SVG-Converter}

In order to convert PPTX or PPT presentations to SVG, we will use [Aspose.Slides for Java][5]. The API is designed to create and manipulate PowerPoint and OpenOffice presentations from within Java applications. Furthermore, it supports the high fidelity conversion of presentations to other formats including SVG. You can either [download][6] the API or install it using the following Maven configurations.

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

## Convert PPTX or PPT Presentations to SVG in Java {#Convert-PPTX-PPT-to-SVG}

The following are the steps to convert a PowerPoint PPTX/PPT presentation to SVG using Java.

*   First, create an instance of [Presentation][7] class to load the presentation.
*   Loop through the slides in presentation and get reference of each slide in [ISlide][8] object.
*   Create a [FileOutputStream][9] object for the output SVG file.
*   Write slide data to the _FileOutputStream_ object using [ISlide.writeAsSvg()][10] method.
*   Finally, close the stream.

The following code sample shows how to convert PowerPoint PPTX/PPT to SVG.

{{< gist aspose-com-gists ae230d0365b5266a24fe1631a3542d15 "powerpoint-to-svg.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][11].

## Online Demo

Try the [online PowerPoint to SVG converter][12], which is based on Aspose.Slides.

## Conclusion

The PowerPoint presentations are often converted to SVG to embed their content in the applications. For such cases, this article covered how to perform PowerPoint to SVG conversion using Java. You can visit the [documentation][13] to explore other features of Aspose.Slides for Java. Furthermore, you can feel free to let us know about your queries via our [forum][14].

## See Also

*   [Create MS PowerPoint Presentations in Java][15]




[1]: https://docs.fileformat.com/page-description-language/svg/
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: #PowerPoint-Presentation-to-SVG-Converter
[4]: #Convert-PPTX-PPT-to-SVG
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[9]: https://docs.oracle.com/javase/7/docs/api/java/io/FileOutputStream.html
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#writeAsSvg-java.io.OutputStream-
[11]: https://purchase.aspose.com/temporary-license
[12]: https://products.aspose.app/slides/conversion/pptx-to-svg
[13]: https://docs.aspose.com/slides/java
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





