---
title: 'Apply 3D Effects in PowerPoint PPT in Java'
date: Fri, 04 Feb 2022 10:28:09 +0000
draft: false
url: /2022/02/04/apply-three-d-effects-in-ppt-in-java/
author: 'Usman Aziz'
summary: "3D effects in PowerPoint are used to make the presentations more attractive and catch users' attention Therefore, you may come across the requirement of adding 3D objects to presentations programmatically. In this article, you will learn **how to create 3D effects in PowerPoint PPT or PPTX in Java**. We will show you how to create 3D text and shapes and apply 3D effects to images."
tags: ['Apply 3D Effects to an Image in PowerPoint Java', 'Create a 3D Shape in PowerPoint in Java', 'Create a 3D Text in PowerPoint in Java', 'Java API to Create 3D Effects in PowerPoint', 'Java PowerPoint Library']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Apply-3D-Effects-in-PowerPoint.psd_.png" alt="Apply 3D Effects in PowerPoint using Java">}}


3D effects in PowerPoint are used to make the presentations more attractive and catch users' attention Therefore, you may come across the requirement of adding 3D objects to presentations programmatically. In this article, you will learn **how to create 3D effects in PowerPoint PPT or PPTX in Java**. We will show you how to create 3D text and shapes and apply 3D effects to images.

*   [Java API to Create 3D Effects in PowerPoint][1]
*   [Create a 3D Text in PowerPoint in Java][2]
*   [Create a 3D Shape in PowerPoint in Java][3]
*   [Set Gradient for 3D Shapes][4]
*   [Apply 3D Effects to an Image in PowerPoint][5]

## Java API to Apply 3D Effects in PowerPoint PPT {#API-to-Create-3D-Effects-in-PowerPoint}

[Aspose.Slides for Java][6] is a powerful API encapsulating a wide range of presentation manipulation features. Using the API, you can create interactive presentations and manipulate existing PPT/PPTX files seamlessly. To create 3D effects in the PowerPoint presentations, we will utilize this API.

You can either [download][7] API’s JAR or install it using the following Maven configurations.

```
**Repository:** <repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:** <dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>22.1</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a 3D Text in PowerPoint in Java {#Create-a-3D-Text-in-PowerPoint}

The following are the steps to create a 3D text fragment in PowerPoint PPT using Java.

*   First, create a new PPT or load existing one using [Presentation][8] class.
*   Then, add a new rectangle shape using [addAutoShape()][9] method.
*   Set shape's properties such as fill type, text, etc.
*   Get reference of the text inside shape into a [Portion][10] object.
*   Apply formatting to the text portion.
*   Get reference of the [TextFrame][11] inside shape.
*   Apply 3D effects using [IThreeDFormat][12] returned by [TextFrame.getTextFrameFormat().getThreeDFormat()][13] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][14] method.

The following code sample shows how to create 3D text in PowerPoint PPT in Java.

{{< gist aspose-com-gists 8d49c40553778f51e27f77372b58e410 "create-3d-text-in-ppt.java" >}}

The following screenshot shows the output of the code sample above.



{{< figure align=center src="images/Create-3D-Text-in-PPT.png" alt="Create a 3D Text in PowerPoint in Java">}}


## Create a 3D Shape in PowerPoint in Java {#Create-a-3D-Shape-in-PowerPoint}

Similar to text, you can apply 3D effects to the shapes in PowerPoint presentations. The following are the steps to create a 3D shape in PowerPoint PPT using Java.

*   First, create a new PPT using [Presentation][15] class.
*   Add a new rectangle shape using [addAutoShape()][16] method.
*   Set shape's text using [IAutoShape.getTextFrame.setText()][17] method.
*   Apply 3D effects to shape using [IThreeDFormat][18] returned by [IAutoShape.getThreeDFormat()][19] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][20] method.

The following code sample shows how to apply 3D effects to shapes in PowerPoint using Java.

{{< gist aspose-com-gists 8d49c40553778f51e27f77372b58e410 "create-3d-shape-in-ppt.java" >}}

The following is the 3D shape that we get after executing this code.



{{< figure align=center src="images/Create-3D-Shape-in-PPT.png" alt="Create a 3D Shape in PowerPoint in Java">}}


## Create Gradient for 3D Shapes {#Set-Gradient-for-3D-Shapes}

You can also apply gradient effects to the shapes following the steps below.

*   First, create a new PPT using [Presentation][21] class.
*   Add a new rectangle shape using [addAutoShape()][22] method.
*   Set shape's text using [IAutoShape.getTextFrame().setText()][23] property.
*   Set fill type of shape to [FillType.Gradient][24] and set gradient colors.
*   Apply 3D effects to shape using [IThreeDFormat][25] returned by [IAutoShape.getThreeDFormat()][26] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][27] method.

The following code sample shows how to apply gradient effects to shapes in a PowerPoint PPT.

{{< gist aspose-com-gists 8d49c40553778f51e27f77372b58e410 "create-3d-shape-gradient-in-ppt.java" >}}

The following is the 3D shape after applying the gradient effect.



{{< figure align=center src="images/Create-3D-Shape-Gradient-in-PPT-Slide.png" alt="Create Gradient for 3D Shapes in PPT in Java">}}


## Apply 3D Effects to an Image in PowerPoint in Java {#Apply-3D-Effect-to-an-Image-in-PowerPoint}

Aspose.Slides for Java also allows you to apply 3D effects to an image. The following are the steps to perform this operation in Java.

*   Create a new PPT using [Presentation][28] class.
*   Add a new rectangle shape using [addAutoShape()][29] method.
*   Set fill type of the shape to [FillType.Picture][30] and add image.
*   Apply 3D effects to shape using [IThreeDFormat][31] returned by [IAutoShape.getThreeDFormat()][32] method.
*   Save presentation using [Presentation.save(String, SaveFormat)][33] method.

The following are the steps to apply 3D effects to an image in PPT using Java.

{{< gist aspose-com-gists 8d49c40553778f51e27f77372b58e410 "create-3d-image-in-ppt.java" >}}

The following is the resultant image that we get after applying 3D effects.



{{< figure align=center src="images/Create-3D-Image-in-PPT.png" alt="Apply 3D Effects to an Image in PowerPoint in Java">}}


## Get a Free License

You can get a [free temporary license][34] to use Aspose.Slides for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to apply 3D effects in PowerPoint PPT/PPTX using Java. With the help of code samples, we have demonstrated how to create 3D text or shapes and apply 3D effects to images in PPT or PPTX presentations. You can visit the [documentation][35] to explore more about Aspose.Slides for Java. Also, you can post your questions or queries to our [forum][36].

## See Also

*   [Extract Text from PowerPoint Files using Java][37]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][38]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][39]




[1]: #API-to-Create-3D-Effects-in-PowerPoint
[2]: #Create-a-3D-Text-in-PowerPoint
[3]: #Create-a-3D-Shape-in-PowerPoint
[4]: #Set-Gradient-for-3D-Shapes
[5]: #Apply-3D-Effect-to-an-Image-in-PowerPoint
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Portion
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/TextFrame
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IThreeDFormat
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IThreeDFormat
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#setText-java.lang.String-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IThreeDFormat
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShape#getThreeDFormat--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#setText-java.lang.String-
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/FillType#Gradient
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/IThreeDFormat
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShape#getThreeDFormat--
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/FillType#Picture
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/IThreeDFormat
[32]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShape#getThreeDFormat--
[33]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[34]: https://purchase.aspose.com/temporary-license
[35]: https://docs.aspose.com/slides/java/
[36]: https://forum.aspose.com/
[37]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[38]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[39]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




