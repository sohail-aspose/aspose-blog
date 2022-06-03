---
title: 'Add or Remove Comments in PowerPoint PPT in Java'
date: Tue, 08 Feb 2022 14:23:00 +0000
draft: false
url: /2022/02/08/add-comments-in-powerpoint-ppt-in-java/
author: 'Usman Aziz'
summary: 'In PowerPoint presentations, the comments are used to write the feedback about the content in the slides. While manipulating PowerPoint PPT/PPTX presentations, you may need to add comments programmatically. In this article, you will learn **how to add comments to PowerPoint PPT slides in Java**. Moreover, we will cover how to read or remove slide comments and add their replies.'
tags: ['Add Comment Replies in PPT Slides in Java', 'Add Comments in PPT Slides in Java', 'Java API to Work with Comments in PowerPoint', 'Read Comments from PPT Slides in Java', 'Remove Comments from Slides in Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Comments-to-PowerPoint-PPT-Slides.png" alt="Add or Remove Comments in PowerPoint PPT in Java">}}


In PowerPoint presentations, the comments are used to write the feedback about the content in the slides. While manipulating PowerPoint PPT/PPTX presentations, you may need to add comments programmatically. In this article, you will learn **how to add comments to PowerPoint PPT slides in Java**. Moreover, we will cover how to read or remove slide comments and add their replies.

*   [Java API to Work with Comments in PowerPoint][1]
*   [Add Comments in PowerPoint Slides][2]
*   [Add Comment Replies in PPT Slides][3]
*   [Read Comments from Slides][4]
*   [Remove Comments from Slides][5]

## Java API to Work with Comments in PowerPoint {#Library-to-Add-Comments-in-PowerPoint-PPT}

[Aspose.Slides for Java][6] is a popular presentation manipulation API that lets you create and modify PowerPoint PPT/PPTX files. We will use this API to manipulate comments in PowerPoint presentations. You can either [download][7] API’s JAR or install it using the following Maven configurations.

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
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add Comments to PowerPoint PPT Slides in Java {#Add-Comments-to-PPT-Slides}

In PowerPoint presentations, every comment is attached to a particular author. Whereas, each comment contains some additional information such as time of creation, slide where it is added, and its position. The following are the steps to add comments to a PPT slide in Java.

*   First, load the presentation file or create a new one using [Presentation][8] class.
*   Add a new author using [Presentation.getCommentAuthors().addAuthor(String, String)][9] method.
*   Get reference of the newly created author in an object.
*   Define the position of the comment.
*   Add comment using [ICommentAuthor.getComments().addComment(String, ISlide, Point2D.Float, Date)][10] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to add comments to PPT slides in Java.

{{< gist aspose-com-gists d334a1c695c4cc3640fe93847cdf0103 "add-comment-in-ppt-slide.java" >}}

The following is the screenshot of the comment we have added using the above code sample.



{{< figure align=center src="images/Add-Comments-to-PPT-Slides.png" alt="Insert Comments to PPT Slides in Java">}}


## Add Comment Replies in PPT Slides in Java {#Add-Comment-Replies-in-PPT-Slides}

Aspose.Slides also allows you to add replies to the comments. A reply itself is a comment which appears as a child of an existing comment. So let's see how to add replies to comments in PowerPoint PPT slides in Java.

*   First, load the presentation file or create a new one using [Presentation][12] class.
*   Add a new author using [Presentation.getCommentAuthors().addAuthor(String, String)][13] method.
*   Add comment using [ICommentAuthor.getComments().addComment(String, ISlide, Point2D.Float, Date)][14] method and get returned object.
*   Insert another comment in the same way and get its reference in an object.
*   Set parent of the second comment using [IComment.setParentComment(IComment)][15] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][16] method.

The following code sample shows how to add replies to comments in a PPTX presentation in Java.

{{< gist aspose-com-gists d334a1c695c4cc3640fe93847cdf0103 "add-comment-reply-in-ppt-slide.java" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Add-Comment-Replies-to-PPT-Slides.png" alt="Add reply to the comments in PPT in Java">}}


## Read Comments in PPT Slides in Java {#Read-Comments-from-PPT-Slides}

Using Aspose.Slides, you can also read comments of a particular author or all the authors. The following are the steps to read comments in PPT slides in Java.

*   Load the presentation file using [Presentation][17] class.
*   Loop through the list of authors using [Presentation.getCommentAuthors()][18] collection.
*   For each author, loop through its comments using [ICommentAuthor.getComments()][19] method.
*   Read and print comment details.

The following code sample shows how to read comments in PPT slides in Java.

{{< gist aspose-com-gists d334a1c695c4cc3640fe93847cdf0103 "read-ppt-slide-comments.java" >}}

## Remove Comments from PowerPoint PPT in Java {#Remove-Comments-in-PowerPoint-PPT}

In the previous section, you have seen how to read a comment by accessing it from the comments collection. Similarly, you can remove a comment after getting its reference. The following code sample shows how to remove comments in PowerPoint presentations in Java.

{{< gist aspose-com-gists d334a1c695c4cc3640fe93847cdf0103 "remove-ppt-slide-comments.java" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][20].

## Conclusion

In this article, you have learned how to add comments in PowerPoint PPT slides in Java. Moreover, we have covered how to add replies to the comments programmatically. In the end, we have demonstrated how to read or remove comments from PPT slides. You can visit the [documentation][21] to explore more about Aspose.Slides for Java. Also, you can post your queries to our [forum][22].

## See Also

*   [Create PowerPoint Presentations using Java][23]
*   [Apply 3D Effects in PowerPoint PPT in Java][24]
*   [Extract Images from PowerPoint PPT in Java][25]
*   [Create and Manipulate Tables in PowerPoint using Java][26]




[1]: #Library-to-Add-Comments-in-PowerPoint-PPT
[2]: #Add-Comments-to-PPT-Slides
[3]: #Add-Comment-Replies-in-PPT-Slides
[4]: #Read-Comments-from-PPT-Slides
[5]: #Remove-Comments-in-PowerPoint-PPT
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICommentAuthorCollection#addAuthor-java.lang.String-java.lang.String-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICommentCollection#addComment-java.lang.String-com.aspose.slides.ISlide-java.awt.geom.Point2D.Float-java.util.Date-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICommentAuthorCollection#addAuthor-java.lang.String-java.lang.String-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICommentCollection#addComment-java.lang.String-com.aspose.slides.ISlide-java.awt.geom.Point2D.Float-java.util.Date-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IComment#setParentComment-com.aspose.slides.IComment-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getCommentAuthors--
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/ICommentAuthor#getComments--
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/slides/java/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[24]: https://blog.aspose.com/2022/02/04/apply-three-d-effects-in-ppt-in-java/
[25]: https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-java/
[26]: https://blog.aspose.com/2021/09/23/manipulate-tables-in-powerpoint-using-java/




