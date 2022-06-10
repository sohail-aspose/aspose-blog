---
title: 'Add Bookmarks with Named Destination and Control loading of External Resources in PDF using Aspose.Cells for .NET 17.9'
date: Mon, 02 Oct 2017 11:48:35 +0000
draft: false
url: /2017/10/02/add-bookmarks-with-named-destination-and-control-loading-of-external-resources-in-pdf-using-aspose.cells-for-.net-17.9/
author: Amjad Sahi
summary: ''
tags: ['Add bookmarks with named destination', 'Copy VBA macro from template', 'named destination in PDF']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.9][1]. This release includes a some valuable features and other enhancements along with critical bug fixes that further improve the overall stability of the APIs. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Add PDF Bookmarks with Named Destinations

Aspose.Cells supports to specify Named Destinations in the output PDF file that do not depend on PDF pages. It means, if pages are added or deleted from PDF, bookmarks may become invalid but named destinations will remain intact. To create Named Destination, please set the **PdfBookmarkEntry.DestinationName** property.

```
//Load source Excel file
Workbook wb = new Workbook("Book1.xlsx");
 
//Access first worksheet
Worksheet ws = wb.Worksheets[0];
 
//Access cell C5
Cell cell = ws.Cells["C5"];
 
//Create Bookmark and Destination for this cell
PdfBookmarkEntry bookmarkEntry = new PdfBookmarkEntry();
bookmarkEntry.Text = "Text";
bookmarkEntry.Destination = cell;
bookmarkEntry.DestinationName = "AsposeCells--" + cell.Name;
 
//Access cell G56
cell = ws.Cells["G56"];
 
//Create Sub-Bookmark and Destination for this cell
PdfBookmarkEntry subbookmarkEntry1 = new PdfBookmarkEntry();
subbookmarkEntry1.Text = "Text1";
subbookmarkEntry1.Destination = cell;
subbookmarkEntry1.DestinationName = "AsposeCells--" + cell.Name;
 
//Access cell L4
cell = ws.Cells["L4"];
 
//Create Sub-Bookmark and Destination for this cell
PdfBookmarkEntry subbookmarkEntry2 = new PdfBookmarkEntry();
subbookmarkEntry2.Text = "Text2";
subbookmarkEntry2.Destination = cell;
subbookmarkEntry2.DestinationName = "AsposeCells--" + cell.Name;
 
//Add Sub-Bookmarks in list
ArrayList list = new ArrayList();
list.Add(subbookmarkEntry1);
list.Add(subbookmarkEntry2);
 
//Assign Sub-Bookmarks list to Bookmark Sub-Entry
bookmarkEntry.SubEntry = list;
 
//Create PdfSaveOptions and assign Bookmark to it
PdfSaveOptions opts = new PdfSaveOptions();
opts.Bookmark = bookmarkEntry;
 
//Save the workbook in Pdf format with given pdf save options
wb.Save("out1.pdf", opts); 
```

Please see the document/article (with attachments) that explains on how to add PDF Bookmarks with Named Destinations for your complete reference.

*   [Add PDF Bookmarks with Named Destinations][4]

## Control loading of External Resources in MS Excel Workbook while rendering to PDF

If your Excel file contains external resources(linked images or objects), so, when you convert your Excel file to Pdf, Aspose.Cells retrieves these external resources and renders them to Pdf file format. Now, if you do not want to load these external resources rather you want to manipulate them, you can do this using **PdfSaveOptions.StreamProvider** API which implements the **IStreamProvider** interface. For more detail, please see this article.

*   [Control loading of External Resources in MS Excel Workbook while rendering to PDF][5]

## Copy VBA Macro UserForm DesignerStorage from Template to Target Workbook

Aspose.Cells allows you to copy VBA project from one Excel file into other. VBA project consists of various types of modules i.e. Document, Procedural, Designer etc. All modules can be copied with simple code but for Designer module, there is some extra data called Designer Storage needs to be accessed or copied. For more detail, please see this article.

*   [Copy VBA Macro UserForm DesignerStorage from Template to Target Workbook][6]

## Send Shape Front or Back inside the Worksheet

Aspose.Cells provides `Shape.ToFrontOrBack()`method which changes the z-order position of the shape. If you want to send shape to back you will use negative number like -1, -2, -3 etc. and if you want to send shape to front, you will use positive number like 1, 2, 3 etc. For more detail, please see this article.

*   [Send Shape Front or Back inside the Worksheet][7]

## Sort Data in Column with Custom Sort List

You can sort data in the column using custom list. This can be done using `DataSorter.AddKey(int key, SortOrder order, String customList)` method. However, this method works only if the items in custom list do not have commas inside them. If they have commas like "USA,US", "China,CN" etc., then you must use `DataSorter.AddKey(int key, SortOrder order, String[] customList)` method. Here the last parameter is not String but Array of Strings. For more detail, please see this article.

*   [Sort Data in Column with Custom Sort List][8]

## Create Remove and Get GridCell Comments

 GridWeb displays comments as Tooltips like MS-Excel does when you hover mouse over the respective cell. The web based grid control provided by Aspose.Cells for .NET allows you to create, remove and get cell comments inside the worksheet. For more detail, please see this article.

*   [Create Remove and Get GridCell Comments][9]

## Other Enhancements and Fixes

There are some other enhancements included in the new release for the users. A few of the worth mentioning features/enhancements are as follow.

*   [Determine which stack size is needed for a certain Workbook][10].
*   Exception: "Too many entries. Consider setting ZipOutputStream.Enable Zip64" on merging the file(s).
*   When RecommendReadOnly is true, IsWriteProtected is also true.
*   Handled NullReferenceException when reading XLSX using LoadFilter containing Pivot Table.
*   Handled "Input string was not in a correct format" exception on opening MS Excel file.

Aspose.Cells 17.9 has enhanced its core for more stability as well as fixed many critical bugs. In this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats, Smart Markers, manipulating ranges, inserting rows and columns, rendering shapes and drawing objects, manipulating OLE Objects, rendering and manipulating charts, manipulating PivotTables, [rendering images from Excel worksheets][11], [rendering images files from charts][12] and [exporting Excel workbooks to PDF format][13] have been resolved.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **LoadStyleStrategy** property, it indicates the strategy to apply style for parsed values when converting string value to number or DateTime.
*   Added class **AbstractCalculationMonitor**, it provides APIs for users to monitor the progress of formula calculations.
*   Added **CalculationMonitor** property, it allows user to provide custom implementation to monitor the progress of formula calculation.
*   Added **DestinationName** property, it gets or sets name of destination. If destination name is set, the destination will be defined as a named destination with this name.
*   Added **AddKey()** method, it adds sorted column index and sort order with custom sort list.
*   Added **ToFrontOrBack()** method, it brings the shape to front or sends it to the back.
*   Added **StreamProvider** property and **ResourceLoadingType** enum, it gets and sets the type of loading external resource.
*   Added **VbaModuleCollection.AddDesignerStorage()** and **GetDesignerStorage()** methods, it gets and sets the designer storage of the VBA project.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][14].
*   [Aspose.Cells for .NET Download Section][15].
*   [Aspose.Cells for .NET Documentation][16] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][18] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][19] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.9/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.9+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Add+PDF+Bookmarks+with+Named+Destinations
[5]: https://docs.aspose.com/display/cellsnet/Control+loading+of+External+Resources+in+MS+Excel+Workbook+while+rendering+to+PDF
[6]: https://docs.aspose.com/display/cellsnet/Copy+VBA+Macro+UserForm+DesignerStorage+from+Template+to+Target+Workbook
[7]: https://docs.aspose.com/display/cellsnet/Send+Shape+Front+or+Back+inside+the+Worksheet
[8]: https://docs.aspose.com/display/cellsnet/Sort+Data+in+Column+with+Custom+Sort+List
[9]: https://docs.aspose.com/display/cellsnet/Create+Remove+and+Get+GridCell+Comments
[10]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+FAQs#Aspose.CellsFAQs-DeterminewhichstacksizeisneededforacertainWorkbook
[11]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[12]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[13]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[14]: https://www.aspose.com/products/cells/net
[15]: https://downloads.aspose.com/cells/net
[16]: https://docs.aspose.com/display/cellsnet/home
[17]: https://apireference.aspose.com/
[18]: https://forum.aspose.com/c/cells
[19]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




