---
title: 'Render HTML with Scalable Column Width using Aspose.Cells for .NET v18.10'
date: Mon, 05 Nov 2018 19:35:42 +0000
draft: false
url: /2018/11/05/render-html-with-scalable-column-width-create-custom-filters-and-get-connection-points-from-shapes-using-aspose.cells-for-.net-v18.10/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.10][1], the MS Excel file formats API that provides the ability to create, manipulate, convert or render MS Excel spreadsheets, and more importantly - is fully documented. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. We have added a few important features while keeping the product more stable and feature rich API. In this release, we have also added some useful enhancements and resolved a number of issues. Sometimes when some bug or issue is reported, that guides us to provide some new feature or enhancement thus making this product more user friendly and capable of solving complex problems in an easier way. Simple features that become quite handy while working with a complex product are added like providing last saved time property for keeping track of changes etc.

Please check the [release notes][3] which cover all the new features, enhancements and list of bugs that are resolved in this new version.

## Scalable Column Width

Depiction of data through the HTML page is very common, however, this page can be opened in a variety of devices including mobiles, tabs, and other handheld devices that contain small screens. The size of the columns is defined in "pt" which works in many cases. However, there can be case where this fixed size may not be required. For example, if the container panel width is 600px where this HTML page is being displayed. In this case, you may get a horizontal scrollbar if the generated table width is bigger. This requirement is addressed by providing scalable units like **em** or **percent** for a better presentation.

For a working example refer to the following article:

*   [Set column width to scalable unit like em or percent][4]

## Handle Self-Closing Tags in HTML

Empty tags are very common while working with HTML like we can face <td></td> or simply <td/>. Earlier self-closing tags were not supported however now this support is provided. Now you can load any HTML with self-closing tags and convert it to an Excel file.

For a working example refer to the following article:

*   [Recognize self-closing tags][5]

## Support for German Locale in Named Range Formulae

Named regions can have English formulae and this file can be used in environments where systems are configured to German locale. There is a need to translate these English formulae completely to the German language for correct usage in MS Excel configured for the German language. This feature is fully functional and can be used without any extra coding.

For a working example along with a template file refer to the following article:

*   [Support German Locale in Named range formulae][6]

## Custom Filter with BeginsWith and EndsWith

MS Excel provides custom filters like filter rows which begins with and ends with some specific string. This feature is available in Aspose.Cells and demonstrated by providing working examples.

For a working example refer to the following article:

*   [Data filtering with custom filter BeginsWith][7]
*   [Data filtering with custom filter EndsWith][8] 

## Get Connection Points from Shapes 

Aspose.Cells provide rich features to manage shapes in the spreadsheet. Sometimes there is a need to get the connection points of a shape for aligning or placing the shapes at the appropriate place. For this purpose, all the connection points are required. The following code can be used to get the list of connection points of a shape where **Shape.GetConnectionPoints()** function is used.

For a working example refer to the following article:

*   [Get connection points from shape][9]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   [Using preferred parser][10]
*   Handled an exception which occurred when loading an Excel file

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

*   Adds **HtmlSaveOptions.WidthScalable property, **Indicates whether using scalable unit to describe the column width when exporting file to HTML. The default value is false.
*   Adds **WorkbookDesigner.UpdateEmptyStringAsNull** property  
    Indicates whether processing the empty string value as null.
*   Updates the returned value of **DocumentProperty.ToDateTime() method, BuiltInDocumentPropertyCollection.CreatedTime, BuiltInDocumentPropertyCollection.LastPrinted and BuiltInDocumentPropertyCollection.LastSavedTime properties **Returns the time in local timezone.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Install Aspose for .NET APIs from NuGet repository][12]
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.10.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.10+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Set+column+width+to+scalable+unit+like+em+or+percent
[5]: https://docs.aspose.com/display/cellsnet/Recognise+self+closing+tags
[6]: https://docs.aspose.com/display/cellsnet/Support+for+German+Locale+in+Named+Range+Formulae
[7]: https://docs.aspose.com/display/cellsnet/Data+Filtering#DataFiltering-CustomfilterwithBeginsWith
[8]: https://docs.aspose.com/display/cellsnet/Data+Filtering#DataFiltering-CustomfilterwithEndsWith
[9]: https://docs.aspose.com/display/cellsnet/Get+Connection+points+from+shape
[10]: https://docs.aspose.com/display/cellsnet/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-Usingpreferredparser
[11]: https://products.aspose.com/cells/net
[12]: https://www.nuget.org/packages/Aspose.Cells
[13]: https://docs.aspose.com/display/cellsnet/home
[14]: https://apireference.aspose.com/
[15]: https://forum.aspose.com/c/cells
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




