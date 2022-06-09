---
title: 'Add Slide Transitions in PowerPoint Presentations using Java'
seoTitle: "Add Slide Transition in PowerPoint using Java | Add Morph Transition"
description: "Use Java PowerPoint API to add slide transitions in PowerPoint presentations using Java. Set morph transition in PowerPoint programmatically."
date: Mon, 06 Sep 2021 14:45:46 +0000
draft: false
url: /2021/09/06/add-slide-transitions-in-powerpoint-using-java/
author: Usman Aziz
summary: 'Slide transitions are used to add visual effects, which occur while moving from one slide to another in a PowerPoint slideshow. You can also set transition sound, speed, duration, and other effects according to the context of your presentation. Accordingly, this article covers **how to add slide transitions in PowerPoint presentations programmatically using Java**.'
tags: ['Add Slide Transition in PowerPoint Java', 'Add Slide Transition using Java', 'Morph Transition in PowerPoint using Java']
categories: ['Aspose.Slides Product Family']
---

Slide transitions are used to add visual effects, which occur while moving from one slide to another in a PowerPoint slideshow. You can also set transition sound, speed, duration, and other effects according to the context of your presentation. Accordingly, this article covers **how to add slide transitions in PowerPoint presentations programmatically using Java**.

*   [Java API to Add Slide Transitions in PowerPoint][1]
*   [Add Slide Transition using Java][2]
*   [Add Advanced Slide Transitions][3]
*   [Morph Transition in PowerPoint][4]

**Info**: Aspose recently implemented transitions effects in its [PowerPoint to Video][5] converter to allow you to create even more stunning and engaging videos based on presentations.

## Java API to Add Slide Transitions in PowerPoint {#API-to-Add-Slide-Transition-in-PowerPoint}

In order to add slide transitions in PPTX/PPT presentations, we will use [Aspose.Slides for Java][6]. The API allows creating and manipulating PowerPoint and OpenOffice presentations. You can either [download][7] the API's JAR or install it using the following Maven configurations.

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

## Add Slide Transition using Java {#Add-Slide-Transition}

The following are the steps to add slide transition in a PowerPoint presentation using Java.

1.  First, load the PowerPoint presentation using [Presentation][8] class.
2.  Then, sset a slide transition type using [SlideShowTransition.setType()][9] method and [TransitionType][10] class.
3.  Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to set the transition of a slide in a PowePoint presentation.

{{< gist aspose-com-gists 3ee2e48fb7d1f2af6b7344e542b980da "add-transition.java" >}}

## Add Advanced Slide Transitions using Java {#Add-Advanced-Slide-Transition}

The following are the steps to set advanced slide transition options such as duration, sound, speed, etc.

1.  First, load the PowerPoint presentation using [Presentation][12] class.
2.  Then, set a slide transition type using [SlideShowTransition.setType()][13] method and [TransitionType][14] class.
3.  Set a advanced effects such as [Sound][15], [AdvanceAfterTime][16], etc. ([see list of effects][17].
4.  Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][18] method.

The following code sample shows how to set advanced slide transition options in a PowerPoint presentation.

{{< gist aspose-com-gists 3ee2e48fb7d1f2af6b7344e542b980da "add-advance-transition.java" >}}

## Set Morph Transition in PowerPoint using Java {#Morph-Transition-in-PowerPoint}

Aspose.Slides for Java also allows setting the morph transitions, which are used to make smooth animations. The following morph transitions are supported by the API:

*   ByObject: Morph transition will be performed considering shapes as indivisible objects.
*   ByWord: Morph transition will be performed with transferring text by words where possible.
*   ByChar: Morph transition will be performed with transferring text by characters where possible.

The following are the steps to add morph transition in a PowerPoint presentation using Java.

1.  First, load the PowerPoint presentation using [Presentation][19] class.
2.  Then, set a slide transition type to [TransitionType.Morph][20] using [SlideShowTransition.setType()][21] method.
3.  Set morph transition type using [IMorphTransition.setMorphType()][22] method.
4.  Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][23] method.

The following code sample shows how to set morph transitions in PowerPoint presentations.

{{< gist aspose-com-gists 3ee2e48fb7d1f2af6b7344e542b980da "add-morph-transition.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][24].

## Conclusion

In this article, you have learned how to add slide transitions in PowerPoint presentations using Java. Moreover, you have seen how to set morph transitions in the PPTX/PPT presentations. Apart from this, you can visit the [documentation][25] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][26].

## See Also

*   [Create MS PowerPoint Presentations in Java][27]
*   [Add Watermark to PowerPoint Slides using Java][28]
*   [Extract Text from PowerPoint Files using Java][29]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][30]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][31]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][32]




[1]: #API-to-Add-Slide-Transition-in-PowerPoint
[2]: #Add-Slide-Transition
[3]: #Add-Advanced-Slide-Transition
[4]: #Morph-Transition-in-PowerPoint
[5]: https://products.aspose.app/slides/video
[6]: https://products.aspose.com/slides/java/
[7]: https://downloads.aspose.com/slides/java/
[8]: https://apireference.aspose.com/slides//java/com.aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition#setType-int-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/TransitionType
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides//java/com.aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition#setType-int-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/TransitionType
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition#setSound-com.aspose.slides.IAudio-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition#setAdvanceAfterTime-long-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition)
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[19]: https://apireference.aspose.com/slides//java/com.aspose.slides/presentation
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/TransitionType
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideShowTransition#setType-int-
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMorphTransition#setMorphType-int-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/slides/java
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[28]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[29]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[30]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[31]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[32]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




