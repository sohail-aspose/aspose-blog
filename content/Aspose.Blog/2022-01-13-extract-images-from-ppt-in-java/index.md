---
title: 'Extract Images from PowerPoint PPT in Java'
seoTitle: "Extract Images from PowerPoint PPT in Java | Source Code"
description: "Use Java PowerPoint library to extract images from PPT/PPTX presentations in Java. Extract images from shapes or slide backgrounds."
date: Thu, 13 Jan 2022 15:46:00 +0000
draft: false
url: /2022/01/13/extract-images-from-ppt-in-java/
author: Usman Aziz
summary: 'In certain cases, you may need to extract images from PowerPoint presentations along with the text. To achieve that, this article covers **how to extract images from PowerPoint [PPT][1] or [PPTX][2] programmatically in Java**. You will also learn how to extract images only from the backgrounds or the shapes in PPT slides.'
tags: ['Extract Images from PowerPoint PPT in Java', 'Extract Images from a PPT in Java', 'Extract Images from a PPTX Presentation in Java', 'Java API to Extract Images from PowerPoint PPT']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Presentations.png" alt="Extract Images from PowerPoint PPT in Java">}}


In certain cases, you may need to extract images from PowerPoint presentations along with the text. To achieve that, this article covers **how to extract images from PowerPoint [PPT][3] or [PPTX][4] programmatically in Java**. You will also learn how to extract images only from the backgrounds or the shapes in PPT slides.

*   [Java API to Extract Images from PowerPoint PPT][5]
*   [Extract Images from a PPT Presentation in Java][6]
*   [Extract Images from Shapes][7]
*   [Image Extraction from Slide Background][8]

## Java API to Extract Images from PowerPoint PPT {#Library-to-Extract-Images-from-Presentations}

[Aspose.Slides for Java][9] is a popular and feature-rich API that allows you to create and manipulate PowerPoint presentations seamlessly. We will use this API for extracting images from PPT/PPTX files. You can either [download][10] API’s JAR or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>22.1</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Extract Images from a PowerPoint PPT in Java {#Extract-Images-from-a-PPTX-Presentation-in-Python}

In PowerPoint presentations, all the images used in the slides are stored in an image collection. This collection can be accessed and each image can be saved as a file. The following are the steps to extract all the images in a PPT presentation in Java.

*   First, use [Presentation][11] class to load the PPT/PPTX presentation.
*   Then, access the image collection in the presentation using [Presentation.getImages()][12] method.
*   Finally, get type and format of each image and save it.

The following code sample shows how to extract images from a PowerPoint PPTX file in Java.

{{< gist aspose-com-gists 06934ffb1e5c49469ed7cca4e80ce1ca "extract-ppt-images.java" >}}

## Extract Images from Shapes in a PPT {#Extract-Images-from-Shapes}

You can also extract images only from the shapes in the PPT slides. The following are the steps to accomplish that.

*   First, use [Presentation][13] class to load the presentation file.
*   Then, use [Presentation.getSlides()][14] method to access slides collection.
*   For each slide, access its shapes using [ISlide.getShapes()][15] method.
*   Perform the following steps for each shape in the collection:
    *   Check if the shape is an auto shape and filled with a picture then extract its image using [getImage()][16] method.
    *   Check if the shape is a picture frame then extract its image using [getImage()][17] method.
    *   Finally, save the image as a file.

The following code sample shows how to extract images from shapes in a PPT using Java.

{{< gist aspose-com-gists 06934ffb1e5c49469ed7cca4e80ce1ca "extract-ppt-shape-images.java" >}}

## Extract Images from Slide Backgrounds in Java {#Image-Extraction-from-Slide-Background}

Another possible scenario could be extracting images that are used only as slide backgrounds. The following steps show how to extract slide background images in Java.

*   First, load the presentation using [Presentation][18] class.
*   Then, loop through the slides in the presentation using [Presentation.getSlides()][19] method.
*   For each slide, perform the following steps:
    
    *   Check if slide has a background image using [ISlide.getBackground().getFillFormat().getFillType()][20] method.
    *   If the background has picture then extract image using [getImage()][21] method.
    *   Check if the layout slide has background image using [ISlide.getLayoutSlide().getBackground().getFillFormat().getFillType()][22] method.
    *   If layout slide's background is filled with a picture then extract it using [getImage()][23] method.
    
    *   Finally, save the extracted image as a file.

The following code sample shows how to extract images from slide backgrounds in a PPT in Java.

{{< gist aspose-com-gists 06934ffb1e5c49469ed7cca4e80ce1ca "extract-ppt-background-images.java" >}}

## Get a Free License

Aspose offers a free temporary license to use Aspose.Slides for Java without evaluation limitations. You can [get one for yourself][24].

## Conclusion

In this article, we have demonstrated how to extract images from PowerPoint PPT/PPTX in Java. In addition, we have covered how to extract images either from the shape or slide backgrounds separately. Besides, you can read more about Aspose.Slides for Java by visiting the [documentation][25]. Also, you can post your queries to our [forum][26].

## See Also

*   [Extract Text from PowerPoint Files using Java][27]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][28]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][29]




[1]: https://docs.fileformat.com/presentation/ppt
[2]: https://docs.fileformat.com/presentation/pptx
[3]: https://docs.fileformat.com/presentation/ppt
[4]: https://docs.fileformat.com/presentation/pptx
[5]: #Library-to-Extract-Images-from-Presentations
[6]: #Extract-Images-from-a-PPTX-Presentation-in-Python
[7]: #Extract-Images-from-Shapes
[8]: #Image-Extraction-from-Slide-Background
[9]: https://products.aspose.com/slides/java
[10]: https://downloads.aspose.com/slides/java
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getImages--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#getImage--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#getImage--
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/IFillFormat#getFillType--
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#getImage--
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IFillFormat#getFillType--
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlidesPicture#getImage--
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/slides/java
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[28]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[29]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




