---
title: 'Add Watermark to PowerPoint Slides using Java'
seoTitle: "Add Watermark to PowerPoint in Java | Add Text or Image Watermark"
description: "Use Java PowerPoint API to add watermark to the PowerPoint presentations using Java. Add text or image watermarks to the slides seamlessly."
date: Sun, 13 Jun 2021 16:57:00 +0000
draft: false
url: /2021/06/13/add-watermark-to-powerpoint-using-java/
author: Usman Aziz
summary: 'Watermarks are commonly used to specify the ownership or to prevent unauthorized usage of the documents. On the other hand, they are also used to display the status of a document such as a manuscript, draft, etc. In this article, you will learn **how to add text or image watermark to PowerPoint slides using Java**.'
tags: ['Add Image Watermark to PowerPoint Slides Java', 'Add Text Watermark to PowerPoint Slides Java', 'Java API to Add Watermark to PowerPoint Slides', 'Java PowerPoint Watermark API']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Watermark-in-PowerPoint.jpg" alt="Add Watermark to PowerPoint Java">}}


Watermarks are commonly used to specify the ownership or to prevent unauthorized usage of the documents. On the other hand, they are also used to display the status of a document such as a manuscript, draft, etc. In this article, you will learn **how to add text or image watermark to PowerPoint slides programmatically using Java**.

*   [Java API to Add Watermark to PowerPoint Slides][1]
*   [Add Text Watermark to PowerPoint Slides][2]
*   [Add Image Watermark to PowerPoint Slides][3]

## Java API to Add Watermark to PowerPoint Slides {#API-to-Add-Watermark-to-PowerPoint-Slides}

For adding watermarks to the PowerPoint slides, we'll use [Aspose.Slides for Java][4]. It is a presentation manipulation API that lets you create and manipulate presentation documents from within the Java applications. You can either [download][5] the API or install it using the following Maven configurations.

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
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add Text Watermark to PowerPoint Slides in Java {#Add-Text-Watermark-to-PowerPoint-Slides}

The following are the steps to add a text watermark to the PowerPoint slides using Java.

*   First, load the PowerPoint presentation using the [Presentation][6] class.
*   Get reference of the slide master in an [IMasterSlide][7] object.
*   Calculate the position of the watermark according to the dimensions of presentation.
*   Add a new auto shape to the Shapes collection of the slide and get its reference in [IAutoShape][8] object.
*   Add text frame to the shape and set its text using [IAutoShape.addTextFrame(string)][9] method.
*   Set font size, color and rotation angle of the watermark.
*   Lock watermark to avoid removal or modification.
*   Finally, save the updated PowerPoint file using [Presentation.save(string, SaveFormat)][10] method.

The following code sample shows how to add a text watermark to the PowerPoint slides.

{{< gist aspose-com-gists e47b38aed78fc79a3803f2fb5b3fc1f3 "add-watermark-to-PowerPoint.java" >}}

### Output

The following is the screenshot of the PowerPoint slide after adding the watermark.



{{< figure align=center src="images/Add-Text-Watermark.jpg" alt="Add Text Watermark To PPT Java">}}


## Add Image Watermark to PowerPoint Slides in Java {#Add-Image-Watermark-to-PowerPoint-Slides}

The following are the steps to add an image watermark to the PowerPoint slides in Java.

*   First, load the PowerPoint presentation using the [Presentation][11] class.
*   Get reference of the slide master in an [IMasterSlide][12] object.
*   Calculate the position of the watermark according to the dimensions of presentation.
*   Add a new auto shape to the Shapes collection of the slide and get its reference in [IAutoShape][13] object.
*   Add image to the presentation and get its reference in [IPPImage][14] object.
*   Set fill type of the _IAutoShape_ to [FillType.Picture][15].
*   Set watermark image using [IAutoShape.getFillFormat().getPictureFillFormat().getPicture().setImage(IPPImage)][16] method.
*   Lock watermark to avoid removal or modification.
*   Finally, save the updated PowerPoint file using [Presentation.save(string, SaveFormat)][17] method.

The following code sample shows how to add an image watermark to PowerPoint slides.

{{< gist aspose-com-gists e47b38aed78fc79a3803f2fb5b3fc1f3 "add-image-watermark-to-PowerPoint.java" >}}

The following is the screenshot of the presentation after adding an image watermark.



{{< figure align=center src="images/Add-Image-Watermark.jpg" alt="Add Image Watermark To PPT Java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][18].

## Try Online

Try the following online watermarking tool which is developed using Aspose.Slides.

*   [Add Watermark to PowerPoint Online][19]
*   [Remove Watermark from PowerPoint Online][20].

## Conclusion

In this article, you have learned how to add a watermark to the PowerPoint slides using Java. The step-by-step guide and code samples have demonstrated how to add text and image watermarks to PowerPoint presentations. Furthermore, you can consult the [documentation][21] to explore other features of the API. Also, you can feel free to let us know about your queries via our [forum][22].

## See Also

*   [Create PowerPoint PPTX Presentation in Java][23]




[1]: #API-to-Add-Watermark-to-PowerPoint-Slides
[2]: #Add-Text-Watermark-to-PowerPoint-Slides
[3]: #Add-Image-Watermark-to-PowerPoint-Slides
[4]: https://products.aspose.com/slides/java
[5]: https://downloads.aspose.com/slides/java
[6]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterSlide
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape#addTextFrame-java.lang.String-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterSlide
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPPImage
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/FillType#Picture
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#setImage-com.aspose.slides.IPPImage-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[18]: https://purchase.aspose.com/temporary-license
[19]: https://products.aspose.app/slides/watermark
[20]: https://products.aspose.app/slides/watermark/remove-watermark
[21]: https://docs.aspose.com/slides/java
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





