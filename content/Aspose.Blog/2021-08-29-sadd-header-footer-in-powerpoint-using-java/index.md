---
title: 'Add Header and Footer in PowerPoint Presentations using Java'
seoTitle: "Add Header and Footer in PowerPoint using Java | Java Source Code"
description: "Use Java PowerPoint API to add header footer in PowerPoint presentation using Java. Manage header and footer in notes slides programmaticaly."
date: Sun, 29 Aug 2021 16:11:00 +0000
draft: false
url: /2021/08/29/sadd-header-footer-in-powerpoint-using-java/
author: Usman Aziz
summary: 'Header and footer in PowerPoint presentations are used to display additional information such as slide number, author, date, etc. In this article, you will learn **how to add and manage the header and footer in PowerPoint PPTX/PPT presentations programmatically using Java**.'
tags: ['Add Header and Footer in PowerPoint Presentation Java', 'Java API to Manage Header and Footer in PowerPoint', 'Manage Header and Footer in Handout and Notes Slide Java']
categories: ['Aspose.Slides Product Family']
---

Header and footer in PowerPoint presentations are used to display additional information such as slide number, author, date, etc. In this article, you will learn **how to add and manage the header and footer in PowerPoint PPTX/PPT presentations programmatically using Java**.

*   [Java API to Manage Header and Footer in PowerPoint][1]
*   [Add Header and Footer in PowerPoint Presentation][2]
*   [Manage Header and Footer in Handout and Notes Slide][3]
    *   [Change Header and Footer Settings for Notes Master][4]
    *   [Change Header and Footer Settings for Notes Slide][5]

## Java API to Manage Header and Footer in PowerPoint {#API-to-Manage-Header-and-Footer-in-PowerPoint}

In order to work with header and footer in PowerPoint presentations, we will use [Aspose.Slides for Java][6]. It is a feature-rich API that lets you create and manipulate PowerPoint and OpenOffice documents. You can either [download][7] the API's JAR or install it via Maven.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>21.9</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add Header and Footer in PowerPoint using Java {#Add-Header-Footer-in-PowerPoint-Presentation}

The following are the steps to add header and footer in a PowerPoint presentation using Java.

*   First, create a new presentation or load an existing one using [Presentation][8] class.
*   Then, set footer using [Presentation.getHeaderFooterManager().setAllFootersText(String)][9] method.
*   Access the master notes slide in an [IMasterNotesSlide][10] object using [Presentation.getMasterNotesSlideManager().getMasterNotesSlide()][11] method.
*   Loop through each shape in [IMasterNotesSlide.getShapes()][12] collection.
*   If [IShape.getPlaceholder().getType()][13] is [PlaceholderType.Header][14] then set text for header using [((IAutoShape)shape).getTextFrame().setText()][15] method.
*   Finally, save the presentation using [Presentation.save(string, SaveFormat)][16] method.

The following code sample shows how to add header and footer in a PowerPoint presentation.

{{< gist aspose-com-gists c531f3ff5dfd7527998af10c5159122a "add-header-footer.java" >}}

## Manage Header and Footer in Handout and Notes Slide using Java {#Add-Header-Footer-in-Handout-and-Notes-Slide}

Aspose.Slides for Java also allows you to set the header and footer in handout and notes slides. For this, you can either apply changes in master notes slide or an individual slide. The following sections cover both scenarios.

### Change Header and Footer Settings for Notes Master {#Change-Header-and-Footer-Settings-for-Notes-Master}

*   First, create a new presentation or load an existing one using [Presentation][17] class.
*   Then, access the master notes slide in an [IMasterNotesSlide][18] object using [Presentation.getMasterNotesSlideManager().getMasterNotesSlide()][19] method.
*   Get reference of [IMasterNotesSlideHeaderFooterManager][20] from [IMasterNotesSlide.getHeaderFooterManager()][21] method.
*   Update the header footer using _IMasterNotesSlideHeaderFooterManager_ object.
*   Finally, save the presentation using [Presentation.save(string, SaveFormat)][22] method.

The following code sample shows how to change header and footer in notes master using Java.

{{< gist aspose-com-gists c531f3ff5dfd7527998af10c5159122a "change-header-footer-notes-master.java" >}}

### Change Header and Footer Settings for Notes Slide {#Change-Header-and-Footer-Settings-for-Notes-Slide}

*   First, create a new presentation or load an existing one using [Presentation][23] class.
*   Then, access [INotesSlide][24] object of desired slide using [Presentation.getSlides().get\_Item(int index).getNotesSlideManager().getNotesSlide()][25] method.
*   Get reference of [INotesSlideHeaderFooterManager][26] from [INotesSlide.getHeaderFooterManager()][27] method.
*   Update the header footer using _INotesSlideHeaderFooterManager_ object.
*   Finally, save the presentation using [Presentation.save(string, SaveFormat)][28] method.

The following code sample shows how to change header and footer in notes slides using Java.

{{< gist aspose-com-gists c531f3ff5dfd7527998af10c5159122a "change-header-footer-notes-slide.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get a free [temporary license][29] to use Aspose.Slides for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to add header and footer in PowerPoint presentations using Java. Moreover, you have seen how to change header and footer in notes slides programmatically. Besides, you can explore the [documentation][30] to learn more about Aspose.Slides for Java. Also, you can ask your questions via our [forum][31].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][32]
*   [Extract Text from PowerPoint Files using Java][33]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][34]




[1]: #API-to-Manage-Header-and-Footer-in-PowerPoint
[2]: #Add-Header-Footer-in-PowerPoint-Presentation
[3]: #Add-Header-Footer-in-Handout-and-Notes-Slide
[4]: #Change-Header-and-Footer-Settings-for-Notes-Master
[5]: #Change-Header-and-Footer-Settings-for-Notes-Slide
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPresentationHeaderFooterManager#setAllFootersText-java.lang.String-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlide
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlideManager#getMasterNotesSlide--
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPlaceholder#getType--
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/PlaceholderType
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#setText-java.lang.String-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlide
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlideManager#getMasterNotesSlide--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlideHeaderFooterManager
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/IMasterNotesSlide#getHeaderFooterManager--
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlide
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager#getNotesSlide--
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideHeaderFooterManager
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlide#getHeaderFooterManager--
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/slides/java
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[33]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[34]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/





