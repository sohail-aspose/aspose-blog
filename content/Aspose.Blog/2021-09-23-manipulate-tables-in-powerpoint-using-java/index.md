---
title: 'Create and Manipulate Tables in PowerPoint using Java'
seoTitle: "Java: Create and Manipulate Tables in PowerPoint | Java PowerPoint API"
description: "Use Java PowerPoint API to create and manipulate tables in PowerPoint presentations using Java. Change formatting and aspect ratio of tables dynamically."
date: Thu, 23 Sep 2021 15:20:22 +0000
draft: false
url: /2021/09/23/manipulate-tables-in-powerpoint-using-java/
author: Usman Aziz
summary: 'Tables are used to well organize the data in the form of rows and columns. Moreover, they summarize the data to be viewed and analyzed easily. MS PowerPoint also allows the presenters to create tables in the presentations. Accordingly, in this article, you will learn **how to create and manipulate tables in PowerPoint presentations using Java**.'
tags: ['Access a Table in a Presentation using Java', 'Create a Table in PowerPoint Presentation Java', 'Format Text in PowerPoint Tables Java', 'Java API to Create and Manipulate Tables in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-Table-in-PowerPoint-1.jpg" alt="Create and Manipulate Tables in PowerPoint Java">}}


Tables are used to well organize the data in the form of rows and columns. Moreover, they summarize the data to be viewed and analyzed easily. MS PowerPoint also allows the presenters to create tables in the presentations. Accordingly, in this article, you will learn **how to create and manipulate tables in PowerPoint presentations using Java**.

*   [Java API to Create and Manipulate Tables in PowerPoint][1]
*   [Create a Table in PowerPoint Presentation][2]
*   [Access a Table in a Presentation using Java][3]
*   [Format Text in PowerPoint Tables][4]
*   [Lock Aspect Ratio of the Tables][5]

## Java API to Create and Manipulate Tables in PowerPoint {#Java-API-to-Create-and-Manipulate-Tables-in-PowerPoint}

To create and manipulate tables in PowerPoint presentations, we will use [Aspose.Slides for Java][6]. The API is designed to create, manipulate and convert PowerPoint and OpenOffice presentations. You can [download][7] the API's JAR or install it using the following Maven configurations.

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

## Create a Table in PowerPoint Presentation using Java {#Create-a-Table-in-PowerPoint-Presentation}

Creating a table using Aspose.Slides for Java is as easy as a pie. The following steps demonstrate how to create a table in a PowerPoint presentation from scratch using Java.

*   First, create a new presentation or load an existing one using [Presentation][8] class.
*   Then, get reference of the desired slide into an [ISlide][9] object.
*   Define the width and height of columns and rows respectively in _double\[\]_ arrays.
*   Insert a new table in presentation using [ISlide.getShapes().addTable(float, float, double\[\], double\[\])][10] method.
*   Get reference of the newly created table in an [ITable][11] object.
*   Create a loop to iterate through the rows of the table.
*   Create a nested loop to iterate through the cells of the table and in each iteration, perform the following operations.
    *   Set text of the cell using [ITable.getRows().get\_Item(rowIndex).get\_Item(cellIndex).getTextFrame().setText(String)][12] method.
    *   Get reference of the cell's formatting into an [ICellFormat][13] object.
    *   Set cell's border style, if required.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][14] method.

The following code sample shows how to create a table in a PowerPoint presentation.

{{< gist aspose-com-gists cb55517c2bd8a4b90ed613889498f270 "create-table.java" >}}

The following screenshot shows the table that we have created using the above code.



{{< figure align=center src="images/Create-Table-in-PowerPoint.jpg" alt="Create Table in PowerPoint Java">}}


## Access a Table in a Presentation using Java {#Access-a-Table-in-a-Presentation-using-Java}

You can also access the tables in the existing PowerPoint presentations and manipulate them as required. The following are the steps to access the tables in a presentation.

*   First, load an existing presentation using [Presentation][15] class.
*   Then, get reference of the desired slide into an [ISlide][16] object.
*   Create an instance of [ITable][17] and initialize it with null.
*   Iterate through all [IShape][18] objects in [ISlide.getShapes()][19] collection.
*   Filter the shapes of type [ITable][20].
*   Type cast the shape into _ITable_ and manipulate it as required.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][21] method.

The following code sample shows how to access tables in a PowerPoint presentation using Java.

{{< gist aspose-com-gists cb55517c2bd8a4b90ed613889498f270 "access-table.java" >}}

## Format Text in PowerPoint Tables using Java {#Format-Text-in-PowerPoint-Tables-using-Java}

Aspose.Slides for Java also allows you to set formatting of the tables quite easily, as demonstrated in the steps below.

*   First, load an existing presentation using [Presentation][22] class.
*   Then, get reference of the desired slide into an [ISlide][23] object.
*   Retreive the reference of the desired table from slide into an instance of [ITable][24] class.
*   Set formatting using [PortionFormat][25], [ParagraphFormat][26], and [TextFrameFormat][27] classes.
*   Assign formatting to the table using _ITable.setTextFormat()_ methods.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][28] method.

The following code sample shows how to set the formatting of the table in PowerPoint using Java.

{{< gist aspose-com-gists cb55517c2bd8a4b90ed613889498f270 "format-table.java" >}}

## Lock Aspect Ratio of Tables in PowerPoint using Java {#Lock-the-Aspect-Ratio-of-the-Tables}

You can also lock the aspect ratio of the tables in PowerPoint presentations using Java. The following are the steps to achieve this.

*   First, load an existing presentation using [Presentation][29] class.
*   Get reference of the desired slide into an [ISlide][30] object.
*   Create a table or retrieve the reference of existing table into an [ITable][31] object.
*   Lock the aspect ratio using _ITable.getGraphicalObjectLock().setAspectRatioLocked(!ITable.getGraphicalObjectLock().getAspectRatioLocked())_ method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][32] method.

The following code sample shows how to lock the aspect ratio of the table in PowerPoint presentations.

{{< gist aspose-com-gists cb55517c2bd8a4b90ed613889498f270 "lock-aspect-ratio.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by getting a free [temporary license][33].

## Conclusion

In this article, you have learned how to create tables in PowerPoint presentations using Java. Moreover, you have seen how to access the tables and set their formatting and aspect ratio programmatically. In addition, you can visit the [documentation][34] to explore more about Aspose.Slides for Java. Also, you can ask your questions via our [forum][35].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][36]
*   [Extract Text from PowerPoint Files using Java][37]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][38]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][39]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][40]




[1]: #Java-API-to-Create-and-Manipulate-Tables-in-PowerPoint
[2]: #Create-a-Table-in-PowerPoint-Presentation
[3]: #Access-a-Table-in-a-Presentation-using-Java
[4]: #Format-Text-in-PowerPoint-Tables-using-Java
[5]: #Lock-the-Aspect-Ratio-of-the-Tables
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addTable-float-float-double:A-double:A-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#setText-java.lang.String-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICellFormat
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShape
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/PortionFormat
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/ParagraphFormat
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/TextFrameFormat
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[32]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[33]: https://purchase.aspose.com/temporary-license
[34]: https://docs.aspose.com/slides/java
[35]: https://forum.aspose.com/
[36]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[37]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[38]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[39]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[40]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




