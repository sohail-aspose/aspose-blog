---
title: 'Apply Theme in PowerPoint Presentations using Java'
seoTitle: "Apply Theme in PowerPoint Presentations using Java | Java API"
description: "Use Java PowerPoint API to apply theme in PowerPoint presentations using Java. Set font, background color, style programmatically."
date: Mon, 16 Aug 2021 05:15:00 +0000
draft: false
url: /2021/08/16/apply-theme-in-powerpoint-using-java/
author: Usman Aziz
summary: 'PowerPoint supports a range of themes that you can apply in the presentations. In addition, you can define your own themes as per your requirements. In this article, you will learn how to use themes in PowerPoint presentations dynamically, Particularly, the article will cover **how to apply themes in the PowerPoint presentations programmatically using Java**.'
tags: ['Change Theme Background Style in Presentation Java', 'Java API to Apply Themes in PowerPoint Presentations', 'Set Theme Color in the Presentation Java', 'Set Theme Font in the Presentation Java']
categories: ['Aspose.Slides Product Family']
---

PowerPoint supports a range of themes that you can use in the presentations. In addition, you can define your own themes as per your requirements. In this article, you will learn how to use themes in PowerPoint presentations dynamically, Particularly, the article will cover **how to apply themes in the PowerPoint presentations programmatically using Java**.

*   [Java API to Apply Themes in PowerPoint Presentations][1]
*   [Apply Theme to a PowerPoint Presentation in Java][2]
    *   [Set Theme Color in the Presentation][3]
    *   [Set Theme Font in the Presentation][4]
    *   [Change Theme Background Style in Presentation][5]

## Java API to Apply Themes in PowerPoint Presentations {#API-to-Apply-Themes-in-PowerPoint-Presentations}

In order to apply themes in PowerPoint presentations, we will use [Aspose.Slides for Java][6]. It is a powerful and feature-rich API to create and manipulate presentations from within Java applications. You can either [download][7] the API or install it using the following Maven configurations.

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

## Apply Theme in a PowerPoint Presentation using Java {#Apply-Theme-to-a-PowerPoint-Presentation}

A PowerPoint theme represents a set of colors, font size, font family, background style, etc. that you can apply to different elements. In the below sections, we will explicitly cover how to set theme color, font, and background in a PowerPoint presentation.

## Set Theme Color in PowerPoint Presentation using Java {#Set-Theme-Color-in-the-Presentation}

The following are the steps to set theme color for a shape in a PowerPoint presentation using Java.

*   First, load a presentation or create a new one using [Presentation][8] class.
*   Then, add a new shape to the presentation using [addAutoShape()][9] method.
*   Set fill type using [IAutoShape.getFillFormat().setFillType()][10] method.
*   Set color using [IAutoShape.getFillFormat().getSolidFillColor().setSchemeColor()][11] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][12] method.

The following code sample shows how to set a theme color in a PowerPoint presentation using Java.

{{< gist aspose-com-gists 9126e502f254c5aa98b378b14215b804 "set-theme-color.java" >}}

## Set Theme Font in the Presentation using Java {#Set-Theme-Font-in-the-Presentation}

Aspose.Slides provides special identifiers to set font from the font scheme. These identifiers are as follows:

*   “**+mn-lt**": Body Font Latin (Minor Latin Font)
*   “**+mj-lt**": Heading Font Latin (Major Latin Font)
*   “**+mn-ea**": Body Font East Asian (Minor East Asian Font)
*   “**+mj-ea**": Body Font East Asian (Minor East Asian Font)

The following are the steps to create an element with the text and assign the Latin font from the font scheme.

*   First, load a presentation or create a new one using [Presentation][13] class.
*   Then, add a new shape to the presentation using [addAutoShape()][14] method.
*   Create a new [Paragraph][15] and add a [Portion][16] into it.
*   Set Latin font using [Portion.getPortionFormat().setLatinFont()][17] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][18] method.

The following code sample shows how to set theme font in a PowerPoint presentation using Java.

{{< gist aspose-com-gists 9126e502f254c5aa98b378b14215b804 "set-theme-font.java" >}}

## Change Theme Background Style in Presentation using Java {#Change-Theme-Background-Style-in-Presentation}

The presentation themes also contain the background styles that you can set in a PowerPoint presentation. The following are the steps to perform this operation.

*   First, load a presentation or create a new one using [Presentation][19] class.
*   Then, set the background style by assigning its index using [Presentation.getMasters().get\_Item(index).getBackground().setStyleIndex()][20] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][21] method.

The following code sample shows how to set theme background style in a presentation.

{{< gist aspose-com-gists 9126e502f254c5aa98b378b14215b804 "set-theme-background.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][22].

## Conclusion

In this article, you have learned how to apply theme color, font, and background style in PowerPoint presentations using Java. You can simply install the API and integrate the provided code into your applications. In addition, you can visit the [documentation][23] to explore more about Aspose.Slides for Java. Also, you can post your queries to our [forum][24].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][25]
*   [Extract Text from PowerPoint Files using Java][26]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][27]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][28]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][29]




[1]: #API-to-Apply-Themes-in-PowerPoint-Presentations
[2]: #Apply-Theme-to-a-PowerPoint-Presentation
[3]: #Set-Theme-Color-in-the-Presentation
[4]: #Set-Theme-Font-in-the-Presentation
[5]: #Change-Theme-Background-Style-in-Presentation
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IFillFormat#setFillType-byte-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IColorFormat#setSchemeColor-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Paragraph
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Portion
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBasePortionFormat#setLatinFont-com.aspose.slides.IFontData-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBackground#setStyleIndex-int-
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/slides/java
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[26]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[27]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[28]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[29]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/





