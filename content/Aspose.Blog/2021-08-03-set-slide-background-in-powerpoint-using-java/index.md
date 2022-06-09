---
title: 'Set Slide Background in PowerPoint Presentations using Java'
seoTitle: "Java Set Slide Background in PowerPoint PPTX PPT | Aspose Java API"
description: "Use Java PowerPoint API to set the slide background color in PowerPoint presentations using Java. Set image as slide background. Java source code."
date: Tue, 03 Aug 2021 06:37:00 +0000
draft: false
url: /2021/08/03/set-slide-background-in-powerpoint-using-java/
author: Usman Aziz
summary: 'In this article, you will learn **how to dynamically set the background of slides in PowerPoint presentations using Java**. More precisely, the article will cover how to set the background of normal slides as well as the master slide.'
tags: ['Gradient as Slide Background Color in Java', 'Set Background Color of Master Slide Java', 'Set Background Color of PowerPoint Slides Java', 'Set Image as Slide Background in PowerPoint using Java']
categories: ['Aspose.Slides Product Family']
---

In this article, you will learn **how to dynamically set the background of slides in PowerPoint presentations using Java**. More precisely, the article will cover how to set the background of normal slides as well as the master slide.

*   [Java API to Set Slide Background in PowerPoint][1]
*   [Set Background Color of Normal Slides][2]
*   [Set Background Color of Master Slide][3]
*   [Gradient as Slide Background Color][4]
*   [Set Image as Slide Background][5]

## Java API to Set Slide Background in PowerPoint {#API-to-Set-Slide-Background-in-PowerPoint}

To set the background of slides in PPTX/PPT presentations, we will use [Aspose.Slides for Java][6]. The API lets you create, manipulate and convert PowerPoint and OpenOffice presentations from within the Java applications. You can either [download][7] the API or install it in your Maven-based applications using the following configurations.

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

## Set Background Color of Normal Slides in Java {#Set-Background-Color-of-Normal-Slides}

The following are the steps to set the background color of the normal slides in a PowerPoint presentation using Java.

*   First, load the PowerPoint presentation using [Presentation][8] class.
*   Then, set the background of the desired slide by specifying its index, e.g. background type, color, fill type, etc.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][9] method.

The following code sample shows how to set the background of a slide in a PowerPoint presentation.

{{< gist aspose-com-gists be3886cf5e87682f17010302fb2da064 "set-slide-background.java" >}}

The screenshot of the slide before setting the background is given below.



{{< figure align=center src="images/Set-PowerPoint-Background.jpg" alt="PowerPoint Presentation">}}


The following is the PowerPoint slide after setting the background.



{{< figure align=center src="images/Set-PPTX-Background.jpg" alt="Set Background of Slide in C#">}}


## Set Background Color of Master Slide in Java {#Set-Background-Color-of-Master-Slide}

You can also set the background of the master slide that will affect all the slides in the presentation. The following are the steps to change the background color of the master slide.

*   First, load the PowerPoint presentation using [Presentation][10] class.
*   Then, set the background of the master slide, e.g. background type, color, fill type, etc.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to change the background of the master slide in PowerPoint.

{{< gist aspose-com-gists be3886cf5e87682f17010302fb2da064 "set-master-slide-background.java" >}}

## Set Gradient Background Color of Slides {#Gradient-as-Slide-Background-Color}

The following are the steps to set a gradient background color of the slides in a PowerPoint presentation.

*   First, load the PowerPoint presentation using [Presentation][12] class.
*   Set [Presentation.getSlides().get\_Item(0).getBackground().setType()][13] to [FillType.Gradient][14].
*   Set [TileFlip][15] to [TileFlip.FlipBoth][16].
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][17] method.

The following code sample shows how to set the gradient background color of the slides in PowerPoint.

{{< gist aspose-com-gists be3886cf5e87682f17010302fb2da064 "set-slide-gradient-background.java" >}}

The following screenshot shows the gradient background of the slide.



{{< figure align=center src="images/Set-PowerPoint-Gradient-Background.jpg" alt="Set Gradient Background of Slide in C#">}}


## Set Image as Slide Background using Java {#Set-Image-as-Slide-Background}

The following are the steps to set an image as a slide background using Java.

*   First, load the PowerPoint presentation using [Presentation][18] class.
*   Set [FillType][19] to [FillType.Picture][20].
*   Set [PictureFillMode][21] to [PictureFillMode.Stretch][22].
*   Add image to the collection of the presentation and get its reference into an [IPPImage][23] object.
*   Set image as background using [setImage(IPPImage)][24] method.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][25] method.

The following code sample shows how to set an image as the background of slides in a PowerPoint presentation.

{{< gist aspose-com-gists be3886cf5e87682f17010302fb2da064 "set-slide-image-background.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][26].

## Conclusion

In this article, you have learned how to set the background of slides in PowerPoint PPTX or PPT using Java. Furthermore, you have seen how to set gradient or image background of the PowerPoint presentations. You can visit the [documentation][27] to explore other features of Aspose.Slides for Java. Also, you can feel free to let us know about your queries via our [forum][28].

## See Also

*   [Create MS PowerPoint Presentations in Java][29]
*   [Add Watermark to PowerPoint Slides using Java][30]
*   [Extract Text from PowerPoint Files using Java][31]




[1]: #API-to-Set-Slide-Background-in-PowerPoint
[2]: #Set-Background-Color-of-Normal-Slides
[3]: #Set-Background-Color-of-Master-Slide
[4]: #Gradient-as-Slide-Background-Color
[5]: #Set-Image-as-Slide-Background
[6]: https://products.aspose.com/slides/java/
[7]: https://downloads.aspose.com/slides/java/
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBackground#setType-byte-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/FillType
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IGradientFormat#setTileFlip-int-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/TileFlip
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IFillFormat#setFillType-byte-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/FillType
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPictureFillFormat#setPictureFillMode-int-
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/PictureFillMode
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPPImage
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#setImage-com.aspose.slides.IPPImage-
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/slides/java
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[30]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[31]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/





