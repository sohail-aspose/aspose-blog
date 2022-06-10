---
title: 'Convert Excel Workbook to Markdown in C#'
date: Mon, 27 May 2019 09:59:01 +0000
draft: false
url: /2019/05/27/convert-excel-to-markdown-xls-xlsx-to-md-in-csharp-asp.net/
author: Amjad Sahi
summary: ''
tags: ['Convert Excel to Markdown in Csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Guys, in the blog you will learn how to use and implement some advanced rather useful features you would like it. Many of you already know there is a new style of comment (called Threaded Comments) introduced in Excel for Office. MS Excel threaded comments allow you to string several comments together, including comments from other users, to form a conversation style thread you will like. Similarly, in various situations you need to insert rows/columns/cells in MS Excel spreadsheets. Aspose.Cells provides you these exciting features and other enhancements. So let's not wait another moment to review the [release notes][1]. Here is an essence of the public release ([Aspose.Cells for .NET v19.4][2], I am giving you a preview of the new features and other enhancements available in it.

## Convert Excel Workbook to Markdown in C#

As you know that **Markdown** is a [lightweight markup language][3] with plain text formatting syntax. Its design allows it to be converted to many output formats, but the original tool by the same name only supports [HTML][4]. Aspose.Cells have introduced a feature to save the cells' content directly as Markdown table. This operation is kept simple by introducing APIs like **SaveFormat.Markdown**, **FileFormatType.Markdown** and **MarkdownSaveOptions**. See the document on how to [Convert Excel Workbook to Markdown][5] for your reference. Following is a sample code that can be used to convert Excel to Markdown in C#.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-LoadingSavingConvertingAndManaging-ConvertExcelFileToMarkdown-1.cs" >}}

## Read Chart Subtitle from ODS File in C#

ODS files can have a subtitle in a chart that is not available in MS Excel (XLS/XLSX) files. As Aspose.Cells mimic the behavior of MS Excel but also supports handling ODS files, so there was an issue rather restriction to access this subtitle through some property. We have resolved this issue now and provided **Chart.SubTitle** property to access this information as shown in the following sample image.



{{< figure align=center src="images/SampleChart.ods_-1024x405.png" alt="">}}


For working sample code and a sample ODS file, please visit the following article:

*   [Read Chart Subtitle from ODS file][6]

## Cut and Paste Cells Data in C#

While working on a spreadsheet one of the useful features is cut a range of cells and paste somewhere else. Earlier this task was performed using multiple statements and in an indirect way. Users were demanding again and again for the implementation of this feature in an easier way. Once again we are pleased to announce that this feature available now in this latest release. It is quite easy to use this feature as you have to just define the range to cut and the destination cell for pasting by providing row and column indexes. Finally, you can select the option to shift the existing cells left, right, up, down or even do not shift the cells as per your needs. Following is a sample code to demonstrate this feature and see the [document][7] for your further reference:

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Worksheets-CutAndPasteCells-1.cs" >}}

## Threaded Comments

You might have worked with the notes in MS Excel sheets however Excel for Office 365 has changed the way comments work. **Comments** are now threaded based, and allow you to have discussions with other people about the data. **Notes** are for making notes or annotations about the data and work like comments used to work in earlier versions of Excel. If we see the difference between Threaded comments and Notes, Threaded Comments have a Reply box. When people reply, you can see several comments connected together, showing a virtual conversation in the workbook. If you need to discuss data with other people, then use a comment. Following is depiction of difference between the two features:



{{< figure align=center src="images/Difference-Between-Comments-and-Notes-1024x593.png" alt="">}}


[Notes][8] functionality was already there in Aspose.Cells. We are happy to share that the rich feature of threaded comments is also implemented by Aspose.Cells in the latest release. You may please visit the article [Threaded Comments][9] for a detailed description of adding, reading, editing, and removing the threaded comments for your reference.

## Web Extensions - Office Add-ins

MS Office document content can be managed in a variety of ways like using Web Extensions also known as Office Add-ins. MS Excel provides options to add web extensions and view information of existing add-ins in the workbook. As this has become a very common phenomenon to use add-ins, therefore Aspose.Cells has also provided the capability to add web extension and access web extension information. **WebExtensionTaskPaneCollection** is added in the Worksheet class which contains all the add-ins in a worksheet. For a detailed demonstration of this feature along with the sample MS Excel files, please visit the article [Web Extension - Office Add-ins][10].

## Other Enhancements and Fixes

*   Support taking white space (char code 20) as the number group separator for the French language.
*   An improvement is made where a large PDF was generated as compared to online tool iLovePDF.
*   Charts do not honor page setup black and white, this issue is fixed.
*   Exporting Excel to PDF does not render Arabic texts precisely in charts - fixed.
*   Support vertical page break for ODS file.
*   Fixed an exception "OutOfMemoryException" while rendering.

To use these useful features and avail other enhancements, I recommend you to try the release [Aspose.Cells for .NET v19.4][11]. And, if you have more time, browse [Developers’ Guide][12] for your complete reference on what you can deliver using the rendering extension API. You are always welcome to share your review, concerns or feedback on [forums][13].




[1]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.4+Release+Notes
[2]: https://www.nuget.org/packages/Aspose.Cells/19.4.0)
[3]: https://en.wikipedia.org/wiki/Lightweight_markup_language
[4]: https://en.wikipedia.org/wiki/HTML
[5]: https://docs.aspose.com/display/cellsnet/Convert+Workbook+to+Different+Formats#ConvertWorkbooktoDifferentFormats-ConvertExcelWorkbooktoMarkdown
[6]: https://docs.aspose.com/display/cellsnet/Read+Chart+Subtitle+from+ODS+File
[7]: https://docs.aspose.com/display/cellsnet/Cut+and+Paste+Cells
[8]: https://docs.aspose.com/display/cellsnet/Managing+Comments
[9]: https://docs.aspose.com/display/cellsnet/Threaded+Comments
[10]: https://docs.aspose.com/display/cellsnet/Web+Extensions+-+Office+Add-ins
[11]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.4/
[12]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[13]: https://forum.aspose.com/c/cells




