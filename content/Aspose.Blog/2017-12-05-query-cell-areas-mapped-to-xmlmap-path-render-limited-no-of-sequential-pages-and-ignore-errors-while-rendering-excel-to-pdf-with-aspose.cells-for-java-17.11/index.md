---
title: 'Query Cell Areas Mapped to XmlMap Path in Excel in Java'
date: Tue, 05 Dec 2017 15:31:51 +0000
draft: false
url: /2017/12/05/query-cell-areas-mapped-to-xmlmap-path-render-limited-no-of-sequential-pages-and-ignore-errors-while-rendering-excel-to-pdf-with-aspose.cells-for-java-17.11/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 17.11][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Find the Root Element Name of XML Map

Aspose.Cells allows you to find the root element name of the XML map using **XmlMap.RootElementName** property.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-XmlMaps-FindRootElementNameOfXmlMap.java" >}}

For more detail, please see this article.

*   [Find the Root Element Name of XML Map][4]

## Query Cell Areas Mapped to Xml Map Path

You can query cell areas mapped to the XML map path with Aspose.Cells using the Worksheet.xmlMapQuery() method. If the path exists, it will return the list of cell areas related to that path inside the XML map. The first parameter of Worksheet.xmlMapQuery() method specifies the XML element path and the second parameter specifies the XML map you want to query.

The following sample code queries the XML map two times and prints the list of cell areas returned by the **Worksheet.xmlMapQuery()** method on console.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-XmlMaps-QueryCellAreasMappedToXmlMapPath.java" >}}

Read more: [Query Cell Areas Mapped to XML Map Path using Worksheet.XmlMapQuery method][5]

## Determine Smart Art Shape and Convert it to Group Shape

Smart Art shapes are special shapes that allow you to create complex diagrams automatically. Aspose.Cells allows you to detect Smart Art shapes and convert them to Group shape that enables you to handle smart art shape like a group shape. Consequently, you will have access to the individual parts or shapes of the group shape.

*   [Determine if Shape is Smart Art Shape][6]
*   [Convert the Smart Art to Group Shape][7]

## Create and Protect a Shared Workbook

Microsoft Excel allows you to create a shared workbook. When you share the workbook, then more than one user can edit the workbook. Aspose.Cells enables you to create a shared workbook with **Workbook.Settings.Shared** property. Besides, you can protect or unprotect a shared workbook.

*   [Create a Shared Workbook with Aspose.Cells][8]
*   [Password Protect or Unprotect the Shared Workbook][9]

## Render Sequence of Pages using PageIndex and PageCount Properties of ImageOrPrintOptions

Aspose.Cells allows you to render a sequence of pages of your Excel file to images using **ImageOrPrintOptions.PageIndex** and **ImageOrPrintOptions.PageCount** properties. These properties are useful when there are so many pages in your worksheet but you need to render a few pages only. This will not only save the processing time but also saves the memory consumption of the rendering process.

*   [Render Sequence of Pages using PageIndex and PageCount Properties of ImageOrPrintOptions][10]

## Ignore Errors while Rendering Excel to PDF

You can ignore all errors during the conversion process using the PdfSaveOptions.IgnoreError property. This way, the conversion process will be completed smoothly without throwing any error or exception but data loss may occur.

*   [Ignore Errors while Rendering Excel to Pdf][11]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][12].
*   [Aspose.Cells for Java Download Section][13].
*   [Aspose.Cells for Java Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/17.11/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.11+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Find+the+Root+Element+Name+of+Xml+Map
[5]: https://docs.aspose.com/display/cellsjava/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method
[6]: https://docs.aspose.com/display/cellsjava/Determine+if+Shape+is+Smart+Art+Shape
[7]: https://docs.aspose.com/display/cellsjava/Convert+the+Smart+Art+to+Group+Shape
[8]: https://docs.aspose.com/display/cellsjava/Create+Shared+Workbook+with+Aspose.Cells
[9]: https://docs.aspose.com/display/cellsjava/Password+Protect+or+Unprotect+the+Shared+Workbook
[10]: https://docs.aspose.com/display/cellsjava/Render+Sequence+of+Pages+using+PageIndex+and+PageCount+Properties+of+ImageOrPrintOptions
[11]: https://docs.aspose.com/display/cellsjava/Ignore+Errors+while+Rendering+Excel+to+Pdf
[12]: https://products.aspose.com/cells/java
[13]: https://downloads.aspose.com/cells/java
[14]: https://docs.aspose.com/display/cellsjava/home
[15]: https://apireference.aspose.com/java/cells
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-Java




