---
title: 'Create SmartArt in PowerPoint Presentations using Java'
seoTitle: "Create SmartArt in PowerPoint Presentations using Java | Source Code"
description: "Use Java PowerPoint API to create SmartArt shapes in PowerPoint presentations using Java. Access and modify SmartArt in PowerPoint programmatically."
date: Sun, 22 Aug 2021 10:57:00 +0000
draft: false
url: /2021/08/22/create-smartart-in-powerpoint-using-java/
author: Usman Aziz
summary: 'In presentations, SmartArt is used to present the information in visual form. Often, the presenters use SmartArt to make the simple text more appealing. Moreover, it is also used to create flow diagrams, processes, relationships between different entities, etc. In this article, you will learn **how to create SmartArt in PowerPoint presentations programmatically using Java**.'
tags: ['Access a SmartArt Shape in PowerPoint Java', 'Change SmartArt Shape Style Java', 'Create a SmartArt Shape in PowerPoint Java', 'Java API to Create SmartArt in PowerPoint']
categories: ['Aspose.Slides Product Family']
---

In presentations, SmartArt is used to present the information in visual form. Often, the presenters use SmartArt to make the simple text more appealing. Moreover, it is also used to create flow diagrams, processes, relationships between different entities, etc. In this article, you will learn **how to create SmartArt in PowerPoint presentations programmatically using Java**.

*   [Java API to Create SmartArt in PowerPoint][1]
*   [Create a SmartArt Shape in PowerPoint][2]
*   [Access a SmartArt Shape in PowerPoint][3]
*   [Change SmartArt Shape's Style][4]

## Java API to Create SmartArt in PowerPoint {#API-to-Create-SmartArt-in-PowerPoint}

In order to manipulate SmartArt in PowerPoint presentations, we will use [Aspose.Slides for Java][5]. It is a powerful library that allows the creation and manipulation of PowerPoint and OpenOffice presentations from scratch. You can either install the API using the following Maven configurations or [download][6] its JAR.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>21.8</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a SmartArt Shape in PowerPoint using Java {#Create-a-SmartArt-Shape-in-PowerPoint}

Aspose.Slides for Java makes it quite easy to create the SmartArt shapes in the presentations. Let's create a simple SmartArt shape from scratch in a PowerPoint presentation using Java.

*   First, create a new presentation or load an existing one using [Presentation][7] class.
*   Get reference of the desired slide into an [ISlide][8] object.
*   Create a [SmartArt][9] using [ISlide.getShapes().addSmartArt()][10] method.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to create a SmartArt shape in a PowerPoint presentation.

{{< gist aspose-com-gists 6a054076684197a0d28101bb2e71b30c "create-smartart.java" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Create-SmartArt-Shape.jpg" alt="">}}


## Access a SmartArt Shape in PowerPoint Presentations {#Access-a-SmartArt-Shape-in-PowerPoint}

You can also access the SmartArt shapes in the existing PowerPoint presentations and update them dynamically. The following are the steps to access the SmartArt shapes in PowerPoint presentations using Java.

*   First, create a new presentation or load an existing one using [Presentation][12] class.
*   Then, get reference of the desired slide into an [ISlide][13] object.
*   Loop through the shapes in the slide using [ISlide.getShapes()][14] collection.
*   If the shape is of type [ISmartArt][15], then get its reference into an _ISmartArt_ object.
*   If required, filter the SmartArt shapes of a specific layout using [ISmartArt.getLayout()][16].

The following code sample shows how to access SmartArt shapes in PowerPoint presentations.

{{< gist aspose-com-gists 6a054076684197a0d28101bb2e71b30c "access-smartart.java" >}}

## Change SmartArt Shape's Style using Java {#Change-SmartArt-Shape-Style}

You can also modify the styles of the SmartArt shapes using Aspose.Slides. The following steps demonstrate how to access the SmartArt shapes in a PowerPoint presentation and change their styles using Java.

*   First, create a new presentation or load an existing one using [Presentation][17] class.
*   Then, get reference of the desired slide into an [ISlide][18] object.
*   Loop through the shapes in the slide using [ISlide.getShapes()][19] collection.
*   If the shape is of type [ISmartArt][20], then get its reference into an _ISmartArt_ object.
*   Change the desired style, i.e. ColorStyle, QuickStyle, etc.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat)][21] method.

The following code sample shows how to change the style of the SmartArt shapes in PowerPoint presentations.

{{< gist aspose-com-gists 6a054076684197a0d28101bb2e71b30c "change-smartart.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Use Aspose.Slides for Java without evaluation limitations by getting a free [temporary license][22].

## Conclusion

In this article, you have learned how to create SmartArt in PowerPoint presentations using Java. Moreover, you have seen how to access the SmartArt shapes and change their styles programmatically. You can explore the [documentation][23] to learn more about Aspose.Slides for Java. In addition, you can ask your questions via our [forum][24].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][25]
*   [Extract Text from PowerPoint Files using Java][26]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][27]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][28]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][29]




[1]: #API-to-Create-SmartArt-in-PowerPoint
[2]: #Create-a-SmartArt-Shape-in-PowerPoint
[3]: #Access-a-SmartArt-Shape-in-PowerPoint
[4]: #Change-SmartArt-Shape-Style
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/SmartArt
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addSmartArt-float-float-float-float-int-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISmartArt
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISmartArt#getLayout--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISmartArt
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/slides/java
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[26]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[27]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[28]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[29]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/





