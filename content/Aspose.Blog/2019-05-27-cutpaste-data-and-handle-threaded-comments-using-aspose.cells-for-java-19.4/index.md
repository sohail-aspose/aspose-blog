---
title: 'Cut/Paste data and handle threaded comments using Aspose.Cells for Java 19.4'
date: Mon, 27 May 2019 11:00:35 +0000
draft: false
url: /2019/05/27/cutpaste-data-and-handle-threaded-comments-using-aspose.cells-for-java-19.4/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="">}}


As you know, Rome wasn't built in one day, similarly, we are achieving new heights by adding more and more features set to Aspose.Cells in each new release. This time we have introduced new features like cut/paste, threaded comments and adding Web extensions. Resolving issues is another constructive phenomenon which takes place in all the releases. I think no more need to extend this startup and let us start reviewing what is there in this [release][1]. Isn't it?

  

## Cut and Paste Cells Data

While working on a spreadsheet one of the most useful features is cut a range of cells and paste somewhere else. Earlier this task was performed using multiple statements and in an indirect way. Users were demanding again and again for the implementation of this feature. Once again we are pleased to announce that this feature available now in this latest release. It is quite easy to use this feature as you have to just define the range to cut and the destination cell for pasting by providing row and column index. Finally, you can select the option to shift the existing cells left, right, up, down or even do not shift the cells. Following is a sample code to demonstrate this feature:

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Worksheets-CutAndPasteCells-1.java" >}}

## Read chart subtitle from ODS file

ODS files can have a subtitle in a chart which is not available in MS Excel files. As Aspose.Cells mimics the behavior of MS Excel but also supports handling ODS files, so there was an issue to access this subtitle through some property. We have resolved this issue now and provided Chart.SubTitle property to access this information as shown in the following sample image.



{{< figure align=center src="images/SampleChart.ods_-1024x405.png" alt="">}}


For working sample code and a sample ODS file, please visit the following article:

[Read Chart Subtitle from ODS file][2]

## Convert Excel Workbook to Markdown

As you know that **Markdown** is a [lightweight markup language][3] with plain text formatting syntax. Its design allows it to be converted to many output formats, but the original tool by the same name only supports [HTML][4]. Aspose.Cells have introduced a feature to save the cells' content directly as Markdown table. This operation is kept simple by introducing APIs like [SaveFormat.Markdown][5], FileFormatType.Markdown and [MarkdownSaveOptions][6]. Following is a sample code which can be used to achieve this functionality.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-ConvertExcelFileToMarkdown-1.java" >}}

## Threaded Comments

You might have worked with the notes in Excel sheets however Excel for Office 365 has changed the way comments work. **Comments** are now threaded, and allow you to have discussions with other people about the data. **Notes** are for making notes or annotations about the data and work like comments used to work in earlier versions of Excel. If we see the difference between Threaded comments and Notes, Threaded Comments have a Reply box. When people reply, you can see several comments connected together, showing a virtual conversation in the workbook. If you need to discuss data with other people, then use a comment. Following is depiction of difference between the two features:



{{< figure align=center src="images/Difference-Between-Comments-and-Notes-1024x593.png" alt="">}}


[Notes][7] functionality was already there in Aspose.Cells. We are happy to share that the rich feature of threaded comments is also implemented by Aspose.Cells in the latest release. You may please visit the article [Threaded Comments][8] for a detailed description of adding, reading, editing and removing the threaded comments.

## Web Extensions - Office Add-ins

Office document content can be managed in a variety of ways like using Web Extensions also known as Office Add-ins. MS Excel provides options to add web extensions and view information of existing add-ins in the workbook. As this has become a very common phenomenon to use add-ins, therefore Aspose.Cells has also provided the capability to add web extension and access web extension information. WebExtensionTaskPaneCollection is added in the Worksheet class which contains all the add-ins in a worksheet. For a detailed demonstration of this feature along with the sample Excel files, please visit the article [Web Extension - Office Add-ins][9].

## Other upgradations

*   When a chart is exported there was an issue that label on both of the axis was not shown in PDF. This issue is sorted out and corrected in this release.
*   Sometimes columns were lost while exporting Excel to PDF, this issue is resolved.
*   Workbook with different page sizes was wrongly converted to PDF and JPG. This is no more an issue now.
*   Sheet names were getting renamed in formulas after CSV import. We have removed this bug now.
*   Issue of reading wrong time from ODS file is gone.
*   The bug of not creating tagged PDF while exporting from Excel to PDF is resolved.

To use these useful features and avail other enhancements, I recommend you to try the release [Aspose.Cells for Java v19.4][10]. And, if you have more time, browse [Developers’ Guide][11] for your complete reference on what you can deliver using the rendering extension API. You are always welcome to share your review, concerns or feedback on [forums][12].




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.4+Release+Notes
[2]: https://docs.aspose.com/display/cellsjava/Read+Chart+Subtitle+from+ODS+File
[3]: https://en.wikipedia.org/wiki/Lightweight_markup_language
[4]: https://en.wikipedia.org/wiki/HTML
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/saveformat#MARKDOWN
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/MarkdownSaveOptions
[7]: https://docs.aspose.com/display/cellsjava/Insert+Cell+Comments
[8]: https://docs.aspose.com/display/cellsjava/Threaded+Comments
[9]: https://docs.aspose.com/display/cellsjava/Web+Extensions+-+Office+Add-ins
[10]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-19.4/
[11]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[12]: https://forum.aspose.com/c/cells




