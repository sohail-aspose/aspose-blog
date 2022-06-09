---
title: 'Apply Animation to Text in PowerPoint using Java'
seoTitle: "Apply Animation to Text in PowerPoint using Java | Get Animation Effect"
description: "Use Java PowerPoint API to apply animation effects to text in PowerPoint presentations in Java. Get the animations effects from the text in PPTX/PPT."
date: Mon, 13 Sep 2021 15:57:24 +0000
draft: false
url: /2021/09/13/apply-animation-to-text-in-powerpoint-using-java/
author: Usman Aziz
summary: "Animated text is used to make the PowerPoint presentations more attractive and draw the audience's attention. Various types of animations are applied to the text and shapes according to the context of the presentation. Accordingly, in this article, you will learn **how to apply animation to the text in PowerPoint using Java**."
tags: ['API to Apply Animation to Text in PowerPoint', 'Apply Animation to Text in PowerPoint Java', 'Get Animation Effects from a Text in PowerPoint Java']
categories: ['Aspose.Slides Product Family']
---

Animated text is used to make the PowerPoint presentations more attractive and draw the audience's attention. Various types of animations are applied to the text and shapes according to the context of the presentation. Accordingly, in this article, you will learn **how to apply animation to the text in PowerPoint using Java**.

*   [API to Apply Animation to Text in PowerPoint][1]
*   [Apply Animation to Text in PowerPoint][2]
*   [Get Animation Effects from a Text in PowerPoint][3]

## Java API to Apply Animation to Text in PowerPoint {#API-to-Apply-Animation-to-Text-in-PowerPoint}

To apply animation to the text in PowerPoint presentations, we will use [Aspose.Slides for Java][4]. The API offers a wide range of features to create and manipulate PowerPoint and OpenOffice presentations. You can either [download][5] the API or install it using the following Maven configurations.

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

## Apply Animation to Text in PowerPoint using Java {#Apply-Animation-to-Text-in-PowerPoint}

Aspose.Slides for Java supports 150+ animation effects, such as Bounce, PathFootball, Zoom, etc. In addition, it provides specific animation effects such as OLEObjectShow and OLEObjectOpen. You can view the complete list of supported animation effects in [EffectType][6] enumeration.

The following are the steps to apply animation to text in a PowerPoint presentation using Java.

*   First, load the presentation using [Presentation][7] class.
*   Then, select the desired paragraph in an [IParagraph][8] object from the desired slide.
*   Apply animation effect to the text using [Presentation.getSlides().get\_Item(index).getTimeline().getMainSequence().addEffect()][9] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][10] method.

The following code sample shows how to apply an animation effect to text in a PowerPoint presentation.

{{< gist aspose-com-gists 720ed0500e080500089dacbb25cb4e4e "apply-text-animation.java" >}}

## Get Animation Effects from a Text in PowerPoint {#Get-Animation-Effects-from-a-Text-in-PowerPoint}

In some cases, you may need to retrieve the information about the animation effect used for a particular piece of text. For example, to use the same effect for some other text in the presentation.

The following are the steps to get information about the animation effect applied to a text.

*   First, load the presentation using [Presentation][11] class.
*   Then, get sequence of the desired slide in [ISequence][12] object.
*   Access the shape from the selected slide in an [IAutoShape][13] object.
*   Loop through each [IParagraph][14] in the collection using [IAutoShape.getTextFrame().get\_Item(index).getParagraphs()][15] method.
*   Finally, get the effects in an [IEffect][16] array using [ISequence.getEffectsByParagraph(iParagraph)][17] method.

The following code sample shows how to get the information about a text's animation effect.

{{< gist aspose-com-gists 720ed0500e080500089dacbb25cb4e4e "get-text-animation.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][18].

## Conclusion

In this article, you have learned how to use animation effects for text in PowerPoint presentations using Java. In addition, the article has also covered how to get animation effects from a text in a PowerPoint presentation. Besides, you can explore other features of Aspose.Slides for Java using [documentation][19]. Also, you can feel free to let us know about your queries via our [forum][20].

## See Also

*   [Create MS PowerPoint Presentations in Java][21]
*   [Add Watermark to PowerPoint Slides using Java][22]
*   [Extract Text from PowerPoint Files using Java][23]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][24]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][25]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][26]




[1]: #API-to-Apply-Animation-to-Text-in-PowerPoint
[2]: #Apply-Animation-to-Text-in-PowerPoint
[3]: #Get-Animation-Effects-from-a-Text-in-PowerPoint
[4]: https://products.aspose.com/slides/java
[5]: https://downloads.aspose.com/slides/java
[6]: https://apireference.aspose.com/slides/java/com.aspose.slides/EffectType
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/IParagraph
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISequence#addEffect-com.aspose.slides.IParagraph-int-int-int-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISequence
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IParagraph
[15]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/paragraphs
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/IEffect
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISequence#getEffectsByParagraph-com.aspose.slides.IParagraph-
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/java
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[22]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[23]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[24]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[25]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[26]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




