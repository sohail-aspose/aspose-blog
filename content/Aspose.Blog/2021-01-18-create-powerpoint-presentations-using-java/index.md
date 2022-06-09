---
title: 'Create PowerPoint Presentations using Java'
seoTitle: "Create PowerPoint PPTX Presentation in Java | Add Text, Tables, Images"
description: "Use Java PowerPoint automation API to create PowerPoint PPTX presentations from scratch in Java. Insert slides, text, tables, and images to slides in Java."
date: Mon, 18 Jan 2021 14:23:00 +0000
draft: false
url: /2021/01/18/create-powerpoint-presentations-using-java/
author: Usman Aziz
summary: 'PowerPoint presentations let you create attractive slide slows containing text, graphics, charts, animations, and other elements to make your presentations appealing. In this article, you are going to learn how to implement PowerPoint automation features using Java. Particularly, you will come to know **how to create PowerPoint presentations and add various elements to the slides using Java**.'
tags: ['Add-Slide-to-a-Presentation', 'Add-Text-to-Presentation-Slide', 'Add-an-Image-to-Presentation', 'Create-a-PowerPoint-Presentation-using-Java', 'Create-a-Table-in-Presentation', 'Java-Presentation-Manipulation-API', 'Open-an-Existing-PowerPoint-Presentation']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-PowerPoint-Presentation.jpg" alt="create powerpoint presentations java">}}


PowerPoint presentations let you create attractive slide slows containing text, graphics, charts, animations, and other elements to make your presentations appealing. In this article, you are going to learn how to implement PowerPoint automation features using Java. Particularly, you will come to know **how to create PowerPoint presentations and add various elements to the slides using Java**.

*   [Java Presentation Manipulation API][1]
*   [Create a PowerPoint Presentation using Java][2]
*   [Open an Existing PowerPoint Presentation][3]
*   [Add Slide to a Presentation][4]
*   [Add Text to Presentation’s Slide][5]
*   [Create a Table in Presentation][6]
*   [Add an Image to Presentation][7]

## Java Presentation Manipulation API {#Java-Presentation-Manipulation-API}

For implementing the PowerPoint automation features, Aspose offers [Aspose.Slides for Java][8] API. The API makes it quite easier for you to create, edit, convert, and manipulate PowerPoint presentations from within your Java applications. You can either [download][9] the API directly or install it within your Maven-based applications using the following configurations.

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
    <version>20.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a PowerPoint Presentation using Java {#Create-a-PowerPoint-Presentation-using-Java}

To begin with the PowerPoint automation, let's first create an empty presentation document and save it as a PPTX file. The following are the steps to create a presentation document.

*   Create an instance of the [Presentation][10] class.
*   Save it as PPTX using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to create a PowerPoint presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "create-powerpoint-presentation.java" >}}

## Open an Existing PowerPoint Presentation using Java {#Open-an-Existing-PowerPoint-Presentation}

Aspose.Slides for Java also allows you to open existing PowerPoint presentations in order to update their content. The following are the steps to load a PowerPoint PPTX file.

*   Create an instance of the [Presentation][12] class and provide the PPTX file's path to its constructor.
*   Update the content of the presentation.
*   Save the updated presentation using [Presentation.save(String, SaveFormat)][13] method.

The following code sample shows how to open an existing PowerPoint presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "open-powerpoint-presentation.java" >}}

## Add Slide to a Presentation using Java {#Add-Slide-to-a-Presentation}

Let's now have a look at how to add slides to a presentation document. This can be done either for a new presentation or an existing one. The following are the steps to add slides to a presentation.

*   Create an instance of the [Presentation][14] class and provide the PPTX file's path to its constructor.
*   Instantiate [ISlideCollection][15] class by setting a reference to the [Presentation.getSlides()][16].
*   Add an empty slide to the presentation using [ISlideCollection.addEmptySlide(ILayoutSlide)][17] method exposed by _ISlideCollection_ object.
*   Save the updated presentation using [Presentation.save(String, SaveFormat)][18] method.

The following code sample shows how to add slides to a presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "add-slide.java" >}}

## Add Text to Presentation Slide using Java {#Add-Text-to-Presentation-Slide}

Once you have created a presentation and added slides to it, you can start inserting different elements into it. First of all, let's have a look at the steps of adding text to a slide using Aspose.Slides for Java.

*   Create an instance of the [Presentation][19] class and provide the PPTX file's path to its constructor.
*   Get the reference of the slide you want to add the text to in the [ISlide][20] object.
*   Add a rectangle using [ISlide.getShapes().addAutoShape()][21] method and get its reference in [IAutoShape][22] object.
*   Add a [TextFrame][23] to the shape containing the default text.
*   Set the properties of the text such as fill color, fill type, etc.
*   Save the updated presentation using [Presentation.save(String, SaveFormat)][24] method.

The following code sample shows how to add text to PowerPoint presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "add-text-in-slide.java" >}}

## Create a Table in Presentation using Java {#Create-a-Table-in-Presentation}

Table is an important element that is used to organize the content in the form of rows and columns. For adding table to a slide, you can following the below steps.

*   Create an instance of the [Presentation][25] class and provide the PPTX file's path to its constructor.
*   Get the reference of the slide you want to add the text to.
*   Create an array of columns’ width.
*   Create an array of rows’ height.
*   Add a Table to the slide using [ISlide.getShapes().addTable()][26] method and get its reference to [ITable][27] object.
*   Iterate through each cell to apply formatting to the Top, Bottom, Right and Left Borders.
*   Add some text to the cell.
*   Save the updated presentation using [Presentation.save(String, SaveFormat)][28] method.

The following code sample shows how to create a table in PowerPoint presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "add-table-in-slide.java" >}}

Learn more about working with tables using [this article][29].

## Add an Image in Presentation using Java {#Add-an-Image-in-Presentation}

The following are the steps to add an image in PowerPoint presentation using Java.

*   Create an instance of the [Presentation][30] class and provide the PPTX file's path to its constructor.
*   Get the reference of the slide in the [ISlide][31] object.
*   Create an object of [IPPImage][32] class.
*   Add image to the presentation using [Presentation.getImages().addImage(FileInputStream)][33] method.
*   Add the image as a picture frame to the slide with the height and width equivalent of the image.
*   Save the updated presentation using [Presentation.save(String, SaveFormat)][34] method.

The following code sample shows how to add image to a PowerPoint presentation using Java.

{{< gist aspose-com-gists 5f98550474ef95055a837ce652e4a328 "add-image-in-slide.java" >}}

**Live example:** Want to see a simple implementation of Aspose APIs? Check out this [online Viewer app][35] used to open and read presentations.

## Conclusion

In this article, you have learned how to create PowerPoint presentations from scratch using Java. Furthermore, the steps and code samples have demonstrated how to insert slides, text, images, and tables in new or existing PPTX presentations. You can explore more about the Java presentation manipulation API using [documentation][36].

## See Also

*   [Convert PowerPoint to PDF using Java][37]




[1]: #Java-Presentation-Manipulation-API
[2]: #Create-a-PowerPoint-Presentation-using-Java
[3]: #Open-an-Existing-PowerPoint-Presentation
[4]: #Add-Slide-to-a-Presentation
[5]: #Add-Text-to-Presentation-Slide
[6]: #Create-a-Table-in-Presentation
[7]: #Add-an-Image-in-Presentation
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addEmptySlide-com.aspose.slides.ILayoutSlide-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/TextFrame
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addTable-float-float-double:A-double:A-
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITable
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[29]: https://docs.aspose.com/slides/java/creating-accessing-and-updating-table-in-a-slide/
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[32]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPPImage
[33]: https://apireference.aspose.com/slides/java/com.aspose.slides/IImageCollection#addImage-java.io.InputStream-
[34]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[35]: https://products.aspose.app/slides/viewer
[36]: https://docs.aspose.com/slides/java/developer-guide/
[37]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/





