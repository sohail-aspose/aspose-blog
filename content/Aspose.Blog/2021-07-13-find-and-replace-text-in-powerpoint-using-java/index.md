---
title: 'Find and Replace Text in PowerPoint PPTX/PPT using Java'
seoTitle: "Java Find and Replace Text in PowerPoint PPTX PPT | Java API"
description: "Use Java PowerPoint API to find and replace text in PowerPoint presentations using Java. Find and replace text in PPTX or PPT presentations."
date: Tue, 13 Jul 2021 23:14:00 +0000
draft: false
url: /2021/07/13/find-and-replace-text-in-powerpoint-using-java/
author: Usman Aziz
summary: 'MS PowerPoint provides a useful feature of finding and replacing text in the presentations. However, you might need automation to perform this operation for a batch of files. Accordingly, in this article, you will learn **how to find and replace text in PowerPoint PPTX/PPT programmatically using Java**.'
tags: ['find and replace text in powerpoint java', 'find and replace text in ppt java', 'find and replace text in pptx java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-PowerPoint.jpg" alt="Java FInd and Replace Text in PowerPoint">}}


MS PowerPoint provides a useful feature of finding and replacing text in the presentations. However, you might need automation to perform this operation for a batch of files. Accordingly, in this article, you will learn **how to find and replace text in PowerPoint PPTX/PPT programmatically using Java**.

*   [API to Find and Replace Text in PowerPoint][1]
*   [Find and Replace Text in PPTX using Java][2]

## Java API to Find and Replace Text in PowerPoint {#API-to-Find-and-Replace-Text-in-PowerPoint}

In order to find and replace text in PPTX/PPT presentations, we'll use [Aspose.Slides for Java][3]. It is a powerful API to create, manipulate, and convert PowerPoint presentations from within your Java applications. You can either [download][4] the API or install it using the following Maven configurations.

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

## Find and Replace Text in PowerPoint PPTX using Java {#Find-and-Replace-Text-in-PPTX}

The following are the steps to find and replace text in a PPTX presentation using Java.

*   First, load the PowerPoint presentation using [Presentation][5] class.
*   Then, loop through each [ISlide][6] in the presentation.
*   In each iteration, get text frames in an [ITextFrame][7] array.
*   For each _ITextFrame_, perform the following operations:
    *   Loop through the [IParagraphCollection][8] in each text frame.
    *   Access the [IPortionCollection][9] in each [IParagraph][10].
    *   Access the text of each [IPortion][11] using [IPortion.getText()][12] method and check if it contains the search string.
    *   If yes, find the position of the search string and replace it using [IPortion.setText()][13] method.
*   Finally, save the updated presentation using [Presentation.save(string, SaveFormat)][14] method.

The following code sample shows how to find and replace text in a PowerPoint presentation.

{{< gist aspose-com-gists cb7908656afd853ddb7164d27bd4ce1b "find-replace-text-in-PowerPoint.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][15].

## Conclusion

In this article, you have learned how to find and replace text in PowerPoint presentations programmatically using Java. You can simply integrate the API and the provided code sample in your Java applications. In addition, you can visit the [documentation][16] to explore other features of Aspose.Slides for Java. Furthermore, you can let us know about your queries via our [forum][17].

## See Also

*   [Create PowerPoint Presentations without MS Office using Java][18]




[1]: #API-to-Find-and-Replace-Text-in-PowerPoint
[2]: #Find-and-Replace-Text-in-PPTX
[3]: https://products.aspose.com/slides/java
[4]: https://downloads.aspose.com/slides/java
[5]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[6]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/IParagraphCollection
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortionCollection
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IParagraph
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortion
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortion#getText--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortion#setText-java.lang.String-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/slides/java
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





