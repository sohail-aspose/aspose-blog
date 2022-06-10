---
title: 'Create, manipulate and render Slicers in MS Excel files using Aspose.Cells for .NET 18.6'
date: Mon, 02 Jul 2018 13:27:46 +0000
draft: false
url: /2018/07/02/create-manipulate-and-render-slicers-in-ms-excel-files-using-aspose.cells-for-.net-18.6/
author: Amjad Sahi
summary: ''
tags: ['Create Excel Slicer in Csharp', 'Create Excel Slicer in Pivot Table', 'Format Excel Slicer']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.6][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. In this release, the long-awaited feature about Slicers is supported. We have also supported to add Microsoft Excel Formula Watch Window for the users. Moreover, we included some important fixes and other enhancements for the users. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Create, manipulate and render Slicers

Slicers are a strong way to filter pivot table data. You can insert slicers into MS Excel to quickly and easily filter pivot tables. Aspose.Cells now supports to create, manipulate and render Slicers in the spreadsheet.

**Creating Slicers into a Pivot Table  
**Please see the following sample code. It loads the sample Excel file that contains the pivot table. It then creates the slicer based on the first base pivot field.

```
// Load sample Excel file containing pivot table.
Workbook wb = new Workbook("sampleCreateSlicerToPivotTable.xlsx");

// Access first worksheet.
Worksheet ws = wb.Worksheets[0];

// Access first pivot table inside the worksheet.
Aspose.Cells.Pivot.PivotTable pt = ws.PivotTables[0];

// Add slicer relating to pivot table with first base field at cell B22.
int idx = ws.Slicers.Add(pt, "B22", pt.BaseFields[0]);

// Access the newly added slicer from slicer collection.
Aspose.Cells.Slicers.Slicer slicer = ws.Slicers[idx];

// Save the workbook in output XLSX format.
wb.Save("outputCreateSlicerToPivotTable.xlsx", SaveFormat.Xlsx);

// Save the workbook in output XLSB format.
wb.Save("outputCreateSlicerToPivotTable.xlsb", SaveFormat.Xlsb); 
```

Please see the following article for more detail on this topic for your reference.

*   [Create Slicer into a Pivot Table][4]

**Manipulating and Formatting Slicers  
**The following sample code loads an Excel file that contains an existing slicer. It un-selects the 2nd and 3rd items of slicer to refresh it. It then applies formatting/style of the slicer and finally describes on how to remove the slicer.

```
// Load sample Excel file containing slicer.
Workbook wb = new Workbook("sampleUpdatingSlicer.xlsx");
 
// Access first worksheet.
Worksheet ws = wb.Worksheets[0];
 
// Access the first slicer inside the slicer collection.
Slicer slicer = ws.Slicers[0];
 
// Access the slicer items.
SlicerCacheItemCollection scItems = slicer.SlicerCache.SlicerCacheItems;
 
// Unselect 2nd and 3rd slicer items.
scItems[1].Selected = false;
scItems[2].Selected = false;
 
// Refresh the slicer.
slicer.Refresh();

// Set the slicer style/formatting.
slicer.StyleType = SlicerStyleType.SlicerStyleLight6;

// Remove slicer.
ws.Slicers.Remove(slicer); 
```

Please see the following articles for more detail for your reference.

*   [Updating Slicer][5]
*   [Formatting Slicer][6]
*   [Removing Slicer][7]

**Rendering Slicers**

Aspose.Cells also supports rendering of slicer shape. When you convert your worksheet into image or save your workbook to PDF or HTML formats, you will see, slicers are rendered properly.

Please see the following articles for more detail for your reference.

*   [Rendering Slicer][8]

## Add cells to Microsoft Excel Formula Watch Window

MS Excel Watch Window is a useful tool to watch the cell values and its formulas conveniently in a window. You can open the Watch Window using Microsoft Excel by clicking the **Formulas > Watch Window**. It has **Add Watch** button that can be used to add the cells for inspection. Similarly, you can use **Worksheet.CellWatches.Add()** method to add cells into Watch Window using Aspose.Cells API. Please see the following article for more detail on this topic for your reference:  

*   [Add Cells to Microsoft Excel Formula Watch Window][9]

## Add Custom XML Parts and select them by ID

Custom XML Parts are the XML data that is stored inside the Microsoft Excel documents and are used by the applications that deal with them. There is no direct way of adding them using Microsoft Excel UI at the moment. However, you can add them programmatically. Please use **Workbook.CustomXmlParts.Add()** method if you want to add Custom XML Part using Aspose.Cells API. Please see the following article for more detail on this topic for your reference:

*   [Add Custom XML Parts and Select them by ID][10]

## Extract text from the Gear type SmartArt shape

Aspose.Cells can extract text from the Gear type Smart Art shape. In order to do so, you should first convert Smart Art shape to group shape. Then you may get the array of all the individual shapes forming the group shape using the **GroupShape.GetGroupedShapes()** method. Finally, you can iterate all of individual shapes one by one in a loop and extract their text using the **Shape.Text** property. Please see the following article for more detail on this topic for your reference:

*   [Extract Text from the Gear Type SmartArt Shape][11]

## Get Address, CellCount Offset, EntireColumn and EntireRow of the Range

Aspose.Cells provides the Range object which has various utility methods to work with Excel Ranges easily:  
**Address** - Gets address of the range.  
**CellCount** - Gets all cell count in the range.  
**GetOffset** - Gets range by offset.  
**EntireColumn** - Gets a Range object that represents the entire column (or columns) that contains the specified range.  
**EntireRow** - Gets a Range object that represents the entire row (or rows) that contains the specified range. Please see the following article for more detail on this topic for your reference:

*   [Get Address Cell Count Offset Entire Column and Entire Row of the Range][12]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Improve converting line Callout to image.
*   WorkbookRender.ToImage(pageIndex, fileName/stream) and Bitmap WorkbookRender.ToImage(int pageIndex) methods included.
*   Support DateTimeOffset format when importing custom objects.
*   Handled EndOfStreamException when Aspose.Cells.Dll (latest assembly) is ilmerged.
*   Exception: "File is corrupted" when loading an XLS file.
*   ArgumentOutOfRangeException when Aspose.Cells (latest assembly) is ilmerged.

In Aspose.Cells 18.6, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, Rendering Excel to HTML and vice versa, manipulating hyperlinks, manipulating ListObject/Tables, rendering and manipulating charts and shapes, manipulating PivotTables, [rendering images from Excel worksheets][13], [rendering images files from charts][14] and [exporting Excel workbooks to PDF format][15] have been resolved in the release.

## Changes to the Public API

We provided some new APIs for supporting to get/set formulas in locale dependent format (the FormulaLocal function of Microsoft Interop):

*   Cell.GetFormula(bool isR1C1, bool isLocal)
*   Cell.SetFormula(string formula, bool isR1C1, bool isLocal, object value)
*   Name.GetRefersTo(bool isR1C1, bool isLocal)
*   Name.SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
*   FormatCondition.GetFormula1(bool isR1C1, bool isLocal)
*   FormatCondition.SetFormula1(string formula, bool isR1C1, bool isLocal)
*   FormatCondition.GetFormula2(bool isR1C1, bool isLocal)
*   FormatCondition.SetFormula2(string formula, bool isR1C1, bool isLocal)
*   FormatCondition.GetFormula1(bool isR1C1, bool isLocal, int row, int column)
*   FormatCondition.GetFormula2(bool isR1C1, bool isLocal, int row, int column)
*   GlobalizationSettings.GetTableRowTypeOfHeaders()
*   GlobalizationSettings.GetTableRowTypeOfData()
*   GlobalizationSettings.GetTableRowTypeOfAll()
*   GlobalizationSettings.GetTableRowTypeOfTotals()
*   GlobalizationSettings.GetTableRowTypeOfCurrent()
*   GlobalizationSettings.GetErrorValueString(string err)
*   GlobalizationSettings.GetBooleanValueString(bool bv)
*   GlobalizationSettings.GetLocalFunctionName(string standardName)
*   GlobalizationSettings.GetStandardFunctionName(string localName)
*   GlobalizationSettings.GetLocalBuiltInName(string standardName)
*   GlobalizationSettings.GetStandardBuiltInName(string localName)
*   GlobalizationSettings.ListSeparator
*   GlobalizationSettings.RowSeparatorOfFormulaArray
*   GlobalizationSettings.ColumnSeparatorOfFormulaArray

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][16].
*   [Install Aspose for .NET APIs from NuGet repository][17]
*   [Aspose.Cells for .NET Documentation][18] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][19] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][20] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][21] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.6.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.6+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Create+Slicer+to+a+Pivot+Table
[5]: https://docs.aspose.com/display/cellsnet/Updating+Slicer
[6]: https://docs.aspose.com/display/cellsnet/Formatting+Slicer
[7]: https://docs.aspose.com/display/cellsnet/Removing+Slicer
[8]: https://docs.aspose.com/display/cellsnet/Rendering+Slicer
[9]: https://docs.aspose.com/display/cellsnet/Add+Cells+to+Microsoft+Excel+Formula+Watch+Window
[10]: https://docs.aspose.com/display/cellsnet/Add+Custom+XML+Parts+and+Select+them+by+ID
[11]: https://docs.aspose.com/display/cellsnet/Extract+Text+from+the+Gear+Type+SmartArt+Shape
[12]: https://docs.aspose.com/display/cellsnet/Get+Address+Cell+Count+Offset+Entire+Column+and+Entire+Row+of+the+Range
[13]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[14]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[15]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[16]: https://products.aspose.com/cells/net
[17]: https://www.nuget.org/packages/Aspose.Cells
[18]: https://docs.aspose.com/display/cellsnet/home
[19]: https://apireference.aspose.com/
[20]: https://forum.aspose.com/c/cells
[21]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




