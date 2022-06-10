---
title: 'Refresh Children Pivot Tables of Parent Pivot Table, Group Pivot Fields in the Pivot Table in Aspose.Cells for Android via Java 18.3'
date: Tue, 03 Apr 2018 18:53:02 +0000
draft: false
url: /2018/04/03/refresh-children-pivot-tables-of-parent-pivot-table-group-pivot-fields-in-the-pivot-table-and-set-margins-of-comment-or-shape-in-aspose.cells-for-android-via-java-18.3/
author: Amjad Sahi
summary: ''
tags: ['Excel API for Android', 'Group pivot table fields', 'Refresh the children of parent pivot tables', 'Work with pivot tables in Excel in Android']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 18.3][1]. This release includes many new features, enhancements and other bug fixes that further improve the overall stability and usability of the API. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a look at the most worth mentioning features in this release.

## Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table

Sometimes, one pivot table uses another pivot table as a data source, so it is called a child pivot table or nested pivot table. You can find the children pivot tables of a parent pivot table using the **PivotTable.getChildren()** method. For more detail, please see the following article.

*   [Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table][4]

The following sample code finds the children pivot tables of the pivot table using the **PivotTable.getChildren()** method and then refreshes them one by one.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "PivotTables-FindAndRefreshNestedOrChildrenPivotTables.java" >}}

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

Early versions of Aspose.Cells were not able to handle automatic units of chart axis properly when the chart is rendered to image or pdf. Now, Aspose.Cells supports the handling of automatic units of the chart axis. There is no code change. Just convert your chart into image or pdf and it will render chart axis just like Microsoft Excel renders it. For more detail, please see the following article.

*   [Handle Automatic Units of Chart Axis like Microsoft Excel][8]

## Create PdfBookmarkEntry for Chart Sheet

Earlier, Aspose.Cells would create **PdfBookmarkEntry** for normal sheet. But now Aspose.Cells can also create PdfBookmarkEntry for chart sheet. Since chart sheet does not have any other cell except cell A1, so it will create PdfBookmarkEntry for cell A1 only. For more detail, please see the following article.

*   [Create PdfBookmarkEntry for Chart Sheet][9]

## Set Margins of Comment or Shape inside the Worksheet

Aspose.Cells allows you to set the margins of any shape or comment using the **Shape.TextBody.TextAlignment** property. This property returns the object of **ShapeTextAlignment** class which has different properties e.g. TopMarginPt, LeftMarginPt, BottomMarginPt, RightMarginPt etc. that can be used to set the top, left, bottom and right margins. For more detail, please see the following article.

*   [Set Margins of Comment or Shape inside the Worksheet][10]

The following code loads the sample Excel file and accesses its shapes one by one and sets their top, left, bottom and right margins.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "DrawingObjects-SetMarginsOfCommentOrShapeInsideTheWorksheet.java" >}}

## Specify Formula Fields while Importing Data to Worksheet

You can specify formula fields when you import data into your worksheet using the **ImportTableOptions.setFormulas()** method. This method takes the Boolean array where the value true means the field is a formula field. For example, if the third field is a formula field, then third value in the array will be true. For more detail, please see the following article.

*   [Specify Formula Fields while Importing Data to Worksheet][11]

## Specify Maximum Rows of Shared Formula

Aspose.Cells provides the **Workbook.Settings.MaxRowsOfSharedFormula** property that can be used to specify the maximum rows of the shared formula. The shared formula will be split into several shared formulas if the total rows of the shared formula are greater than it. For more detail, please see the following article.

*   [Specify Maximum Rows of Shared Formula][12]

## Control External Resources using WorkbookSetting.StreamProvider

Sometimes, your Excel file contains external resources e.g. linked images, etc. Aspose.Cells allows you to control these external resources using Workbook.Settings.StreamProvider takes the implementation of **IStreamProvider** interface. Whenever you will try to render your worksheet containing external resources e.g. linked images, the methods of the IStreamProvider interface will be invoked which will enable you to take appropriate actions for your external resources. For more detail, please see the following article.

*   [Control External Resources using WorkbookSetting.StreamProvider][13]

## Filter Defined Names while loading Workbook

Aspose.Cells allows you to filter or remove defined names present inside the workbook. Please use **LoadDataFilterOptions.DEFINED\_NAMES** to load defined names and use **~LoadDataFilterOptions.DEFINED\_NAMES** to remove them while loading the workbook. Please note, if you will remove defined names, then formulas inside the workbook may break up. For more detail, please see the following article.

*   [Filter Defined Names while loading Workbook][14]

## Group Pivot Fields in the Pivot Table

Microsoft Excel allows you to group pivot fields in the Pivot Table. When there is a large amount of data related to a pivot field, it is better to group them into sections. Aspose.Cells provides this feature via the **PivotTable.setManualGroupField()** method. This was a long-awaited feature requested by many users. The following sample code loads the template Excel file and performs grouping operation on the first pivot field in the Pivot Table using the **PivotTable.setManualGroupField()** method.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "PivotTables-GroupPivotFieldsInPivotTable.java" >}}

Please see the following article for more detail on how to group pivot fields in the Pivot Table for your reference.

*   [Group Pivot Fields in the Pivot Table][15]

## Get DrawObject and Bound while rendering to PDF using DrawObjectEventHandler class

Aspose.Cells provides an abstract class **DrawObjectEventHandler** which has a **draw()** method. Users can implement DrawObjectEventHandler and utilize the draw() method to get the DrawObject and Bound while rendering Excel to Pdf or Image. If you are rendering an Excel file to Pdf, then you can utilize the DrawObjectEventHandler class with **PdfSaveOptions.DrawObjectEventHandler**. Similarly, if you are rendering an Excel file to Image, you can utilize DrawObjectEventHandler class with **ImageOrPrintOptions.DrawObjectEventHandler**. The following sample code explains the usage of DrawObjectEventHandler class with the PdfSaveOptions.DrawObjectEventHandler.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Rendering-GetDrawObjectAndBoundUsingDrawObjectEventHandler.java" >}}

Please see the following article for more detail about this feature.

*   [Get DrawObject and Bound while rendering to Pdf using DrawObjectEventHandler class][16]

## Export similar Border Style when Border Style is not supported by Web Browsers

Microsoft Excel also supports dashed border types which are not supported by most web browsers. When you convert such an Excel file into HTML using Aspose.Cells, the borders are removed. However, Aspose.Cells allows you to accomplish the task and supports to display such borders with **HtmlSaveOptions.ExportSimilarBorderStyle** property. For more detail on the feature, please see this article for your reference.

*   [Export similar Border Style when Border Style is not supported by Web Browsers][17]

## Find if the Worksheet is Dialog Sheet

Dialog sheet is an older format that contains a dialog box. You can find if a sheet is a dialog or some other type with **Worksheet.Type** property. If it returns enumeration value SheetType.DIALOG, then it means, you are dealing with the Dialog sheet. For more detail, please see this article.

*   [Find if the Worksheet is Dialog Sheet][18]

## Access and modify the display label of the linked Ole Object

Microsoft Excel allows you to change the display label of the Ole Object. You can also access or modify the display label of the Ole object via Aspose.Cells APIs using the **OleObject.Label** property. Please see the following article with sample code and attachments explaining how to access and modify the display label of the linked Ole Object for your reference.

*   [Access and Modify the Display Label of the Linked Ole Object][19]

## Preserve Single Quote Prefix of Cell Value or Range

When you put some value inside a cell that has leading apostrophe or single quote mark, then Microsoft Excel hides it, but when you select the cell, it displays the leading apostrophe or single quote in a formula bar. Aspose.Cells provides **StyleFlag.QuotePrefix** property that will handle either preserving the quote or not preserving the quote for your needs. For more detail, please see this article.

*   [Preserve single quote prefix of cell value or range][20]

## Read Axis Labels after Calculating the Chart

You can read axis labels of your chart after calculating its values using the **Chart.calculate()** method. Please use the **Axis.AxisLabels** property for this purpose that will return the list of axis labels. For more detail, please see the following article.

*   [Read Axis Labels after Calculating the Chart][21]

## Specify Document Version of the Excel File using BuiltIn Document Properties

You can change the **Version number** of Excel file by right-clicking the file and then selecting **Properties > Details** and then editing the Version number field. Please use **BuiltInDocumentPropertyCollection.DocumentVersion** property to change it programmatically using Aspose.Cells APIs. For more detail, please see the following article.

*   [Specify Document Version of the Excel File using BuiltIn Document Properties][22]

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][23].
*   [Aspose.Cells for Android via Java Download Section][24].
*   [Aspose.Cells for Android via Java Documentation][25] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][26] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][27] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][28] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][29] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.3/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+18.3+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Find+and+Refresh+the+Nested+or+Children+Pivot+Tables+of+Parent+Pivot+Table
[5]: https://docs.aspose.com/display/cellsjava/Parsing+Pivot+Cached+Records+while+loading+Excel+file
[6]: https://docs.aspose.com/display/cellsjava/Export+Document+Workbook+and+Worksheet+Properties+in+Excel+to+HTML+conversion
[7]: https://docs.aspose.com/display/cellsjava/Exclude+Unused+Styles+during+Excel+to+HTML+conversion
[8]: https://docs.aspose.com/display/cellsjava/Handle+Automatic+Units+of+Chart+Axis+like+Microsoft+Excel
[9]: https://docs.aspose.com/display/cellsjava/Create+PdfBookmarkEntry+for+Chart+Sheet
[10]: https://docs.aspose.com/display/cellsjava/Set+Margins+of+Comment+or+Shape+inside+the+Worksheet
[11]: https://docs.aspose.com/display/cellsjava/Specify+Formula+Fields+while+Importing+Data+to+Worksheet
[12]: https://docs.aspose.com/display/cellsjava/Specify+Maximum+Rows+of+Shared+Formula
[13]: https://docs.aspose.com/display/cellsjava/Control+External+Resources+using+WorkbookSetting.StreamProvider
[14]: https://docs.aspose.com/display/cellsjava/Filter+Defined+Names+while+loading+Workbook
[15]: https://docs.aspose.com/display/cellsjava/Group+Pivot+Fields+in+the+Pivot+Table
[16]: https://docs.aspose.com/display/cellsjava/Get+DrawObject+and+Bound+while+rendering+to+Pdf+using+DrawObjectEventHandler+class
[17]: https://docs.aspose.com/display/cellsjava/Export+similar+Border+Style+when+Border+Style+is+not+supported+by+Web+Browsers
[18]: https://docs.aspose.com/display/cellsjava/Find+if+the+Worksheet+is+Dialog+Sheet
[19]: https://docs.aspose.com/display/cellsjava/Access+and+Modify+the+Display+Label+of+the+Linked+Ole+Object
[20]: https://docs.aspose.com/display/cellsjava/Preserve+Single+Quote+Prefix+of+Cell+Value+or+Range
[21]: https://docs.aspose.com/display/cellsjava/Read+Axis+Labels+after+Calculating+the+Chart
[22]: https://docs.aspose.com/display/cellsjava/Specify+Document+Version+of+the+Excel+File+using+BuiltIn+Document+Properties
[23]: https://www.aspose.com/products/cells/android-java
[24]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.3/
[25]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[26]: https://apireference.aspose.com/java/cells
[27]: https://forum.aspose.com/c/cells
[28]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[29]: https://github.com/asposecells/Aspose_Cells_Java




