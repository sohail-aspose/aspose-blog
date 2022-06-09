---
title: 'Add, Connect, Remove, or Clone PowerPoint Shapes in Java'
seoTitle: "Work with PowerPoint Shapes in Java | Add Remove Clone Shapes in PPT"
description: "Use Java API to work with shapes in PowerPoint presentations. Add, remove, connect and clone PowerPoint shapes from within your Java applications."
date: Fri, 09 Apr 2021 18:32:00 +0000
draft: false
url: /2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
author: Usman Aziz
summary: 'Shapes in PowerPoint presentations are used to elaborate a particular point or create diagrams such as flowcharts. Also, the inclusion of shapes makes the presentation more appealing. Therefore, PowerPoint provides a number of shapes such as line, ellipse, rectangle, etc. In this article, you will learn how to automate the manipulation of shapes in PowerPoint presentations. Particularly, the article will cover **how to add, connect, clone, or remove shapes in PowerPoint presentations using Java**.'
tags: ['Add Connector to Shapes in PowerPoint Slides in Java', 'Add Shape to PowerPoint Slides in Java', 'Clone a Shape in PowerPoint Slides in Java', 'Java API to Work with PowerPoint Shapes', 'Remove Shapes from PowerPoint Slides in Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Work-with-Shapes-in-Slides-in-C-1024x578.jpg" alt="Work with PowerPoint shapes in Java">}}


Shapes in PowerPoint presentations are used to elaborate a particular point or create diagrams such as flowcharts, etc. Moreover, the inclusion of shapes makes the presentation more appealing. Therefore, PowerPoint provides a number of shapes such as line, ellipse, rectangle, etc. In this article, you will learn how to automate the manipulation of shapes in PowerPoint presentations. Particularly, the article will cover **how to add, connect, clone, or remove shapes in PowerPoint presentations using Java**.

*   [Java API to Work with PowerPoint Shapes][1]
*   [Types of PowerPoint Shapes][2]
*   [Add Shape to PowerPoint Slides][3]
*   [Add Connector to Shapes in PowerPoint Slides][4]
*   [Clone a Shape in PowerPoint Slides][5]
*   [Remove Shapes from PowerPoint Slides][6]
*   [Get a Free API License][7]

## Java API to Work with PowerPoint Shapes {#Java-API-to-Work-with-PowerPoint-Shapes}

In order to work with PowerPoint shapes, we'll use [Aspose.Slides for Java][8]. It is a powerful Java API that lets you manipulate PowerPoint presentations seamlessly. Particularly, the API allows you to create, modify, read, and convert the presentation documents. You can either [download][9] the API or get it installed using the following Maven configuration.

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
    <version>21.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Types of PowerPoint Shapes {#Types-of-PowerPoint-Shapes}

PowerPoint supports a variety of shapes that you can add to the presentation slides. Accordingly, Aspose.Slides for Java supports the following shape types:

*   [Connector][10]
*   [Ellipse][11]
*   [Flash][12]
*   [Group][13]
*   [Image][14]
*   [Line][15]
*   [Paragraph][16]
*   [Picture Frame][17]
*   [Portion][18]
*   [Rectangle][19]
*   [and etc.][20]

## Add Shape to PowerPoint Slides in Java {#Add-Shape-to-PowerPoint-Slides}

Aspose.Slides for Java provides [ShapeType][21] class to specify the type of shape you want to add. The following are the steps to add a particular shape in a PowerPoint presentation using Java.

*   First, create an instance of the [Presentation][22] class to create a new or load an existing PowerPoint presentation.
*   Get the reference of the slide into an [ISlide][23] object.
*   Add shape using [ISlide.getShapes().addAutoShape(ShapeType.Ellipse, float, float, float, float)][24] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][25] method.

The following code sample shows how to add a shape to a PowerPoint presentation using Java.

{{< gist aspose-com-gists 0e0e4646fe91c0791330665370d31edb "add-shape.java" >}}

The following is the output you will get after executing this code.



{{< figure align=center src="images/Add-PowerPoint-Shape.jpg" alt="Add PowerPoint shape in Java">}}


## Add Connector between PowerPoint Shapes using Java {#Add-Connector-to-Shapes-in-PowerPoint-Slides}

The connector is a line that is used to join two shapes. Moreover, a connector could be a straight or a curved line. The following are the steps to add a connector between two PowerPoint shapes.

*   First, create an instance of the [Presentation][26] class to load the presentation.
*   Get collection of the shapes into an [IShapeCollection][27] object using [Presentation.getSlides().get\_Item(0).getShapes()][28] method.
*   Add two shapes using [IShapeCollection.addAutoShape(ShapeType.Ellipse, float, float, float, float)][29] method and get their references in [IAutoShape][30] objects.
*   Create a connector using [IShapeCollection.addConnector(ShapeType.BentConnector2, float, float, float, float)][31] method and get its reference into [IConnector][32] object.
*   Join the shapes using [IConnector.setStartShapeConnectedTo(IAutoShape)][33] and [IConnector.setEndShapeConnectedTo(IAutoShape)][34] methods.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][35] method.

The following code sample shows how to add connector between two shapes in PowerPoint using Java.

{{< gist aspose-com-gists 0e0e4646fe91c0791330665370d31edb "connect-shape.java" >}}

The following is the screenshot of the PowerPoint presentation after connecting the shapes.



{{< figure align=center src="images/Connect-PowerPoint-Shapes.jpg" alt="Connect PowerPoint shapes in Java">}}


## Clone a PowerPoint Shape using Java {#Clone-a-Shape-in-PowerPoint-Slides}

You can also clone a PowerPoint shape to create its copy. The following are the steps to perform this operation.

*   First, create an instance of the [Presentation][36] class to create a new or load an existing PowerPoint presentation.
*   Get the reference of the slide into an [ISlide][37] object.
*   Get the shape collection into [IShapeCollection][38] object using [Presentation.getSlides().get\_Item(0).getShapes()][39] method.
*   Add clone of a shape using [IShapeCollection.addClone(sourceShapes\[int\])][40] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][41] method.

The following code sample shows how to add clone of a PowerPoint shape using Java.

{{< gist aspose-com-gists 0e0e4646fe91c0791330665370d31edb "clone-shape.java" >}}

## Remove Shapes from PowerPoint Slides in Java {#Remove-Shapes-from-PowerPoint-Slides-in-Java}

You can also remove the PowerPoint shapes from a slide using Aspose.Slides for Java. The following are the steps to remove a PowerPoint shape from the shape collection.

*   First, create an instance of [Presentation][42] class to load a PowerPoint presentation.
*   Get the reference of the desired slide into an [ISlide][43] object.
*   Remove particular shape by index using [ISlide.getShapes().removeAt(int)][44] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][45] method.

The following code sample shows how to remove a PowerPoint shape from a slide using Java.

{{< gist aspose-com-gists 0e0e4646fe91c0791330665370d31edb "remove-shape.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][46] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to work with shapes in PowerPoint presentations using Java. Particularly, you have seen how to add, connect, remove or clone the PowerPoint shapes. Furthermore, you can explore more about the API by consulting its [documentation][47]. Also, in case of any queries, feel free to let us know via our [forum][48].

## See Also

*   [Create PowerPoint Presentations using Java][49]




[1]: #Java-API-to-Work-with-PowerPoint-Shapes
[2]: #Types-of-PowerPoint-Shapes
[3]: #Add-Shape-to-PowerPoint-Slides
[4]: #Add-Connector-to-Shapes-in-PowerPoint-Slides
[5]: #Clone-a-Shape-in-PowerPoint-Slides
[6]: #Remove-Shapes-from-PowerPoint-Slides-in-Java
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://docs.aspose.com/slides/java/connector/
[11]: https://docs.aspose.com/slides/java/ellipse/
[12]: https://docs.aspose.com/slides/java/flash/
[13]: https://docs.aspose.com/slides/java/group/
[14]: https://docs.aspose.com/slides/java/image/
[15]: https://docs.aspose.com/slides/java/line/
[16]: https://docs.aspose.com/slides/java/paragraph/
[17]: https://docs.aspose.com/slides/java/picture-frame/
[18]: https://docs.aspose.com/slides/java/portion/
[19]: https://docs.aspose.com/slides/java/rectangle/
[20]: https://docs.aspose.com/slides/java/powerpoint-shapes/
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/ShapeType
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addConnector-int-float-float-float-float-
[32]: https://apireference.aspose.com/slides/java/com.aspose.slides/IConnector
[33]: https://apireference.aspose.com/slides/java/com.aspose.slides/IConnector#setStartShapeConnectedTo-com.aspose.slides.IShape-
[34]: https://apireference.aspose.com/slides/java/com.aspose.slides/IConnector#setEndShapeConnectedTo-com.aspose.slides.IShape-
[35]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[36]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[37]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[38]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection
[39]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[40]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addClone-com.aspose.slides.IShape-
[41]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[42]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[43]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[44]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#removeAt-int-
[45]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[46]: https://purchase.aspose.com/temporary-license
[47]: https://docs.aspose.com/slides/java/getting-started/
[48]: https://forum.aspose.com/
[49]: https://blog.aspose.com/2021/01/18/Create-PowerPoint-Presentations-using-Java/





