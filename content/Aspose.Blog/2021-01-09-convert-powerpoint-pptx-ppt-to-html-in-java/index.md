---
title: 'Convert PowerPoint PPTX/PPT to HTML in Java'
seoTitle: "Convert PowerPoint to HTML in Java | PPT to HTML | PPTX to HTML"
description: "Convert PowerPoint PPTX or PPT presentations to HTML using Java. Include or exclude hidden slides in PPTX/PPT to HTML conversion in Java."
date: Sat, 09 Jan 2021 14:24:00 +0000
draft: false
url: /2021/01/09/convert-powerpoint-pptx-ppt-to-html-in-java/
author: Usman Aziz
summary: 'PowerPoint PPTX/PPT to HTML conversion could be useful when you need to embed the presentations within your web pages. Since PowerPoint files can not be displayed directly within the web applications, you can adopt PowerPoint to HTML conversion for creating slide shows. In accordance with that, this article covers **how to convert slides in PowerPoint presentations to HTML using Java**.'
tags: ['Java PowerPoint to HTML converter', 'PPT to HTML Java', 'PPTX to HTML Java', 'PowerPoint to HTML Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-HTML-1.jpg" alt="PPTX to HTML Java">}}


PowerPoint PPTX/PPT to HTML conversion could be useful when you need to embed the presentations within your web pages. Since PowerPoint files can not be displayed directly within the web applications, you can adopt PowerPoint to HTML conversion for creating slide shows. In accordance with that, this article covers **how to convert slides in PowerPoint presentations to HTML using Java**.

*   [Java PowerPoint to HTML Converter API][1]
*   [Convert PowerPoint PPTX to HTML in Java][2]
*   [PPT/PPTX to HTML Conversion with Hidden Slides][3]
*   [Get a Free API License][4]

## Java PowerPoint to HTML Converter API {#Java-PowerPoint-to-HTML-Converter-API}

For PowerPoint to HTML conversion, we will use [Aspose.Slides for Java][5]. It is a powerful presentation manipulation API that lets you create, manipulate, and convert PowerPoint files quite easily. You can either [download][6] the API or install it via Maven.

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
    <artifactId>aspose-slides</artifactId>
    <version>21.1</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert PowerPoint PPTX to HTML in Java {#Convert-PowerPoint-PPTX-to-HTML-in-Java}

The following are the steps to convert PowerPoint PPTX or PPT files to HTML using Java.

*   First, load the PowerPoint presentation you want to convert using the [Presentation][7] class.
*   Create an object of [HtmlOptions][8] class.
*   Convert PPTX to HTML using [Presentation.save(String, Int, HtmlOptions)][9] method.

The following code sample shows how to convert a PowerPoint presentation to HTML using Java.

{{< gist aspose-com-gists dadff50427de821c9fbb5dddaf81a528 "pptx-to-html.java" >}}

## Java PPTX to HTML Conversion with Hidden Slides {#PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides}

PowerPoint also allows you to hide the desired slides within a presentation. By default, Aspose.Slides for Java do not include hidden slides in the PowerPoint to HTML conversion. However, you can customize this behavior of the API. The following are the steps to include hidden slides in conversion.

*   Load the PPTX/PPT presentation you want to convert using the [Presentation][10] class.
*   Create an object of [HtmlOptions][11] class.
*   Include hidden slides using [HtmlOptions.setShowHiddenSlides(true)][12] method.
*   Convert PPTX to HTML using [Presentation.save(String, Int, HtmlOptions)][13] method.

The following code sample shows how to include hidden slides in PowerPoint to HTML conversion using Java.

{{< gist aspose-com-gists dadff50427de821c9fbb5dddaf81a528 "pptx-to-html-hidden-slides.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Aspose offers [a free temporary license][14] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX or PPT presentations to HTML using Java. Furthermore, you have seen how to include hidden slides in PowerPoint to HTML conversion. You can learn more about the Java presentation manipulation API using [documentation][15].

## See Also

*   [Create PowerPoint Presentations using Java][16]




[1]: #Java-PowerPoint-to-HTML-Converter-API
[2]: #Convert-PowerPoint-PPTX-to-HTML-in-Java
[3]: #PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/HtmlOptions
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-com.aspose.slides.ISaveOptions-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/HtmlOptions
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/HtmlOptions#setShowHiddenSlides-boolean-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-com.aspose.slides.ISaveOptions-
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/slides/java/
[16]: https://blog.aspose.com/2021/01/18/Create-PowerPoint-Presentations-using-Java/





