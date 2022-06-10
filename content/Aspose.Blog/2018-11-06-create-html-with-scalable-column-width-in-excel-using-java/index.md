---
title: 'Create HTML with Scalable Column Width in Excel using Aspose.Cells for Java v18.10'
date: Tue, 06 Nov 2018 14:10:19 +0000
draft: false
url: /2018/11/06/create-html-with-scalable-column-width-in-excel-using-java/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


It is announced with gratification that new updated version [Aspose.Cells for Java v18.10][1] is released. As usual it contains lot of enhancements, bug fixes and new features as well. We put effort to greater extent to make our product easy to use and error free by working hard on all the issues which are reported by the vast developers community. Similarly sometimes when some bug or issue is reported, that guides us to provide some new feature or enhancement thus making this product more user friendly and capable of solving complex problems in an easier way. Simple features which become quite handy while working with a complex product are added like providing last saved time property for keeping track of changes etc. New features are always introduced for enhancing this product which helps us to compete the ever growing software industry. 

[Release notes][2] is an important document containing detailed overview of all the new features, bugs which are resolved in this version and list of enhancements as well.  Performance is always a major concern while working with third party tools, hence we take care of it as well like developers were facing little performance hit while working with conditional formatting. This issue is addressed and performance is improved as much as possible. You may go through the release notes to have a glimpse of all the changes in this new version. For more details about this product you may visit the links in the last section of this document. For an easy access and utilization, Aspose for Java APIs can be directly installed from Maven repository for which check [document][3].

## Scalable Column Width in Excel Worksheets

Depiction of data through HTML page is very common, however this page can be opened in variety of devices including mobiles, tabs and other hand held devices which contain small screens. The size of the columns is defined in "pt" which works in many cases. However there can be case where this fixed size may not be required. For example if container panel width is 600px where this HTML page is being displayed. In this case you may get horizontal scrollbar if the generated table width is bigger. This requirement is addressed by providing scalable units like em or percent for a better presentation.  

For a working example refer to the following article:

*   [Set column width to scalable unit like em or percent][4]

## Handle Self-Closing Tags in HTML

Empty tags are very common while working with HTML like we can face <td></td> or simply <td/>. Earlier self-closing tags were not supported however now this support is provided. Now you can load any HTML with self-closing tags and convert it to Excel file.

For a working example refer to the following article:

*   [Recognise self closing tags][5]

## Support for German Locale in Named Range Formulae

Named regions can have English formulae and this file can be used in environments where  systems are configured to German Locale. There is need to translate these English formulae completely to German language for correct usage in Excel configured for German language. This feature is fully functional and can be used without any extra coding.

For a working example along with a template file refer to the following article:

*   [Support German Locale in Named range formulae][6]

## Custom Filter with BeginsWith and EndsWith

Excel provides custom filters like filter rows which begins with and ends with some specific string. This feature is available in Aspose.Cells and demonstrated by providing working examples.

For a working example refer to the following article:

*   [Data filtering with custom filter BeginsWith][7]
*   [Data filtering with custom filter EndsWith][8] 

## Get Connection Points from Shapes 

Aspose.Cells provide rich features to manage shapes in the spreadsheet. Sometimes there is need to get the connection points of a shape for aligning or placing the shapes at appropriate place. For this purpose all the connection points are required. Following code can be used to get the list of connection points of a shape where Shape.GetConnectionPoints() function is used.

For a working example refer to the following article:

*   [Get connection points from shape][9]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Convert left right ribbon shape to image
*   An exception(StackOverFlow) raises when saving to PDF output
*   Copy a range with PasteType.ALL (Paste options) not copying row heights properly
*   Invalid Russian date format output
*   Exception "java.lang.OutOfMemoryError: Java heap space" when rendering MS Excel file to PDF
*   Quotes appear in formula when retrieving the cell formula via Aspose.Cells
*   Performance degradation when using conditional formatting 

In Aspose.Cells 18.10, we fixed several important bugs and other issues. For example, wrong calculation done by ROUNDUP(), losing the hyperlink text formatting while setting the new text and resolving the issue pf fonts while rendering sheets with SheetRender.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

*   Adds **HtmlSaveOptions.WidthScalable property, **Indicates whether using scalable unit to describe the column width when exporting file to HTML. The default value is false.
*   Adds **WorkbookDesigner.UpdateEmptyStringAsNull** property  
    Indicates whether processing the empty string value as null.
*   Updates the returned value of **DocumentProperty.ToDateTime() method, BuiltInDocumentPropertyCollection.CreatedTime, BuiltInDocumentPropertyCollection.LastPrinted and BuiltInDocumentPropertyCollection.LastSavedTime properties **Returns the time in local timezone.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][10].
*   [Download Aspose.Cells for Java][11].
*   [Aspose.Cells for Java Documentation][12] – up-to-date documentation containing Programmer’s Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Java API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.10/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.10+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[4]: https://docs.aspose.com/display/cellsjava/Set+column+width+to+scalable+unit+like+em+or+percent
[5]: https://docs.aspose.com/display/cellsjava/Recognise+self+closing+tags
[6]: https://docs.aspose.com/display/cellsjava/Support+for+German+Locale+in+Named+Range+Formulae
[7]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-CustomfilterwithBeginsWith
[8]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-CustomfilterwithEndsWith
[9]: https://docs.aspose.com/display/cellsjava/Get+Connection+points+from+shape
[10]: https://products.aspose.com/cells/java
[11]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[12]: https://docs.aspose.com/display/cellsjava/home
[13]: https://apireference.aspose.com/java/cells
[14]: https://forum.aspose.com/c/cells
[15]: https://github.com/aspose-cells/Aspose.Cells-for-Java




