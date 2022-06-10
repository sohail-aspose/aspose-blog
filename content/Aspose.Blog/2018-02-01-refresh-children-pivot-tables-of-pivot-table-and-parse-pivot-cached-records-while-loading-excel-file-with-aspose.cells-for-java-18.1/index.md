---
title: 'Refresh Children Pivot Tables of Pivot Table and Parse Pivot Cached Records while loading Excel file with Aspose.Cells for Java 18.1'
date: Thu, 01 Feb 2018 12:55:45 +0000
draft: false
url: /2018/02/01/refresh-children-pivot-tables-of-pivot-table-and-parse-pivot-cached-records-while-loading-excel-file-with-aspose.cells-for-java-18.1/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Excel pivot tables', 'Parse pivot table cache in java', 'Pivot table cache records in java', 'children pivot tables in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 18.1][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table

Sometimes, one pivot table uses other pivot table as a data source, so it is called a child pivot table or nested pivot table. You can find the children pivot tables of a parent pivot table using the **PivotTable.getChildren()** method. For more detail, please see the following article.

*   [Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table][4]

The following sample code finds the children pivot tables of the pivot table using the **PivotTable.getChildren()** method and then refreshes them one by one.

```
//Load sample Excel file
Workbook wb = new Workbook("sampleRefreshChildrenPivotTables.xlsx");

//Access first worksheet
Worksheet ws = wb.getWorksheets().get(0);

//Access third pivot table
PivotTable ptParent = ws.getPivotTables().get(2);

//Access the children of the parent pivot table
PivotTable[] ptChildren = ptParent.getChildren();

//Refresh all the children pivot table
int count = ptChildren.length;
for (int idx = 0; idx < count; idx++)
{
	//Access the child pivot table
	PivotTable ptChild = ptChildren[idx];

	//Refresh the child pivot table
	ptChild.refreshData();
	ptChild.calculateData();
}
```

## Parsing Pivot Cached Records while loading Excel file

When you create a Pivot Table, Microsoft Excel takes a copy of the source data and stores it in the Pivot Cache. The Pivot Cache is held inside the memory of Microsoft Excel. When you load your Excel file inside the Workbook object, you can decide whether you also want to load the records of Pivot Cache or not, using the **LoadOptions.ParsingPivotCachedRecords** property. The default value of this property is false. If Pivot Cache is quite big, it can increase the performance. For more detail, please see the following article.

*   [Parsing Pivot Cached Records while loading Excel file][5]

## Export Document, Workbook and Worksheet Properties in Excel to HTML conversion

When Microsoft Excel file is exported to HTML using Microsoft Excel or Aspose.Cells APIs, it also exports various types of Document, Workbook and Worksheet properties. You can avoid exporting these properties by setting the **HtmlSaveOptions.ExportDocumentProperties**, **HtmlSaveOptions.ExportWorkbookProperties** and **HtmlSaveOptions.ExportWorksheetProperties** as false. The default value of these properties is true. For more detail, please see the following article.

*   [Export Document, Workbook and Worksheet Properties in Excel to HTML conversion][6]

## Exclude unused Styles during Excel to HTML conversion

Microsoft Excel file may contain many unnecessary unused styles. When you export the Excel file to HTML file format, these unused styles are also exported. This could increase the size of HTML. You can exclude the unused styles during the conversion of Excel file to HTML using the **HtmlSaveOptions.ExcludeUnusedStyles** property. For more detail, please see the following article.

*   [Exclude Unused Styles during Excel to HTML conversion][7]

## Handle Automatic Units of Chart Axis like Microsoft Excel

Early versions of Aspose.Cells were not able to handle automatic units of chart axis properly when chart is rendered to image or pdf. Now, Aspose.Cells supports the handling of automatic units of chart axis. There is no code change. Just convert your chart into image or pdf and it will render chart axis just like Microsoft Excel renders it. For more detail, please see the following article.

*   [Handle Automatic Units of Chart Axis like Microsoft Excel][8]

## Create PdfBookmarkEntry for Chart Sheet

Earlier, Aspose.Cells would create **PdfBookmarkEntry** for normal sheet. But now Aspose.Cells can also create PdfBookmarkEntry for chart sheet. Since, chart sheet does not have any other cell except cell A1, so it will create PdfBookmarkEntry for cell A1 only. For more detail, please see the following article.

*   [Create PdfBookmarkEntry for Chart Sheet][9]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][10].
*   [Aspose.Cells for Java Download Section][11].
*   [Aspose.Cells for Java Documentation][12] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.1/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.1+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Find+and+Refresh+the+Nested+or+Children+Pivot+Tables+of+Parent+Pivot+Table
[5]: https://docs.aspose.com/display/cellsjava/Parsing+Pivot+Cached+Records+while+loading+Excel+file
[6]: https://docs.aspose.com/display/cellsjava/Export+Document+Workbook+and+Worksheet+Properties+in+Excel+to+HTML+conversion
[7]: https://docs.aspose.com/display/cellsjava/Exclude+Unused+Styles+during+Excel+to+HTML+conversion
[8]: https://docs.aspose.com/display/cellsjava/Handle+Automatic+Units+of+Chart+Axis+like+Microsoft+Excel
[9]: https://docs.aspose.com/display/cellsjava/Create+PdfBookmarkEntry+for+Chart+Sheet
[10]: https://products.aspose.com/cells/java
[11]: https://downloads.aspose.com/cells/java
[12]: https://docs.aspose.com/display/cellsjava/home
[13]: https://apireference.aspose.com/java/cells
[14]: https://forum.aspose.com/c/cells
[15]: https://github.com/aspose-cells/Aspose.Cells-for-Java




