---
title: 'Auto-Populate Smart Markers Data to Other Worksheets and Export Worksheet CSS Separately in Output HTML using Aspose.Cells for .NET 17.12'
date: Thu, 28 Dec 2017 14:56:05 +0000
draft: false
url: /2017/12/28/auto-populate-smart-markers-data-to-other-worksheets-and-export-worksheet-css-separately-in-the-output-html-using-aspose.cells-for-.net-17.12/
author: Amjad Sahi
summary: ''
tags: ['.NET Excel API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.12][1]. There are quite a few useful enhancements included for HTML and PDF renderings. Moreover, you can now auto-populate data against Smart Markers to split to other sheets. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Auto-Populate Smart Markers Data to Other Worksheets

While using the Smart Markers feature, you might need to auto-populate data to other worksheets when it too large to be handled in a single worksheet. For example, your data source has 1500000 records. Since the data is large, so you can paste your desired data set in the first worksheet while the rest of the records to the next worksheet. The following sample code uses a data source that has 21 records in total. We will show only 15 records in the first worksheet, then the rest of the records will be automatically moved to the second worksheet. Please note, the second worksheet should also have the same smart marker tag (as first) and you must call **WorkbookDesigner.Process(sheetIndex, isPreserved)** method for both sheets.

```
//Create employees data tableDataTable dt = new DataTable("Employees");
dt.Columns.Add("EmployeeID", typeof(int)); 
//Add rows inside the data tabledt.Rows.Add(1230);
dt.Rows.Add(1231);
dt.Rows.Add(1232);
dt.Rows.Add(1233);
dt.Rows.Add(1234);
dt.Rows.Add(1235);
dt.Rows.Add(1236);
dt.Rows.Add(1237);
dt.Rows.Add(1238);
dt.Rows.Add(1239);
dt.Rows.Add(1240);
dt.Rows.Add(1241);
dt.Rows.Add(1242);
dt.Rows.Add(1243);
dt.Rows.Add(1244);
dt.Rows.Add(1245);
dt.Rows.Add(1246);
dt.Rows.Add(1247);
dt.Rows.Add(1248);
dt.Rows.Add(1249);
dt.Rows.Add(1250); 
//Create data reader from data tableDataTableReader dtReader = dt.CreateDataReader(); 
//Create empty workbookWorkbook wb = new Workbook(); 
//Access first worksheet and add smart marker in cell 
A1Worksheet ws = wb.Worksheets[0];
ws.Cells["A1"].PutValue("&=Employees.EmployeeID"); 
//Add second worksheet and add smart marker in cell 
A1wb.Worksheets.Add();
ws = wb.Worksheets[1];
ws.Cells["A1"].PutValue("&=Employees.EmployeeID"); 
//Create workbook designer
WorkbookDesigner wd = new WorkbookDesigner(wb); 
//Set data source with data readerwd.SetDataSource("Employees", dtReader, 15); 
//Process smart marker tags in first and second worksheetwd.Process(0, false);wd.Process(1, false); 
//Save the workbookwb.Save("outputAutoPopulateSmartMarkerDataToOtherWorksheets.xlsx"); 
```

Please see the documents/articles with attachment(s) on how to auto-populate Smart Markers data to other worksheets if data is too large.

*   [Auto Populate Smart Marker Data to Other Worksheets if Data is too Large][4]

## Export Worksheet CSS Separately in Output HTML

Aspose.Cells provides the feature to export worksheet CSS separately when you convert your Excel file to HTML file format. Please use **HtmlSaveOptions.ExportWorksheetCSSSeparately** property for this purpose and set it to true while saving Excel file to HTML format. For more detail on the feature, please see this article/document for your reference.

*   Export Worksheet CSS Separately in Output HTML

## Implement Cell.FormulaLocal Similar to Excel VBA Range.FormulaLocal

Microsoft Excel formulas may have different names in different locales/regions or languages. For example, SUM function is called SUMME in German. Aspose.Cells cannot work with non-English function names. In Microsoft Excel VBA, there is **Range.FormulaLocal** property that returns the name of the function as per its language or region. Aspose.Cells also provides **Cell.FormulaLocal** property for this purpose. However, this property will only work when you will implement **GlobalizationSettings.GetLocalFunctionName(string standardName)** method. For more detail, please see this article.

*   [Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal][5]

## Prefix Table Elements Styles with HtmlSaveOptions.TableCssId Property

Aspose.Cells allows you to prefix table elements styles with **HtmlSaveOptions.TableCssId** property. For more detail, please see this article.

*   [Prefix Table Elements Styles with HtmlSaveOptions.TableCssId property][6]

## Render Office Add-Ins while Converting Excel to PDF

Aspose.Cells now supports to render MS Office Add-ins (in Excel files) in the output PDF. You do not need to use any special method or property to render Office Add-Ins in the output PDF. For more detail, please see this article.

*   [Render Office Add-Ins while converting Excel to Pdf][7]

## Set the Shape Type of Data Labels of Chart

You can change the shape type of data labels of the chart using the **DataLabels.ShapeType** property. It takes the value of **DataLabelShapeType** enumeration and changes the shape type of data labels accordingly. For more detail, please see this article.

*   [Set the Shape Type of Data Labels of Chart][8]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other enhancements are as follows.

*   [Text overflows in GridDesktop cell if it is too long][9].
*   [Update Days Preserving History of Revision Logs in Shared Workbook][10].
*   Handled Shape to Image error that occurred while converting an Excel file to PDF.
*   Handled an exception on opening an Excel (Strict Open XML Spreadsheet) file.
*   Handled ArgumentOutOfRangeException that occurred when worksheet is copied to another workbook.

In Aspose.Cells 17.12 we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, copying range of cells, displaying worksheet in right to left, rendering Excel to HTML and vice versa, rendering shapes and drawing objects, rendering and manipulating charts, manipulating and refreshing PivotTables, [rendering images from Excel worksheets][11], [rendering images files from charts][12] and [exporting Excel workbooks to PDF format][13] have been resolved. The Aspose.Cells formula calculation engine is also reviewed and enhanced.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **HtmlSaveOptions.TableCssId** property,  it gets and sets the prefix of the type css name.
*   Added **Cell.FormulaLocal** property, it gets the local formatted formula which may vary according to different locale settings for separators, built in Names, function names, etc.
*   Added **GlobalizationSettings.GetLocalFunctionName(string standardName)** method, it gets the locale dependent function name according to given standard function name.
*   Added **HtmlSaveOptions.ExportWorksheetCSSSeparately** property, it indicates whether exporting the worksheet css separately. The default value is false.
*   Added **WorksheetCollection.RevisionLogs** property, **RevisionLogCollection** class and **Revisions.RevisionLog** class, it gets setting of revision log.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][14].
*   [Aspose.Cells for .NET Download Section][15].
*   [Aspose.Cells for .NET Documentation][16] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][18] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][19] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.12/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.12+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Auto+Populate+Smart+Marker+Data+to+Other+Worksheets+if+Data+is+too+Large
[5]: https://docs.aspose.com/display/cellsnet/Implement+Cell.FormulaLocal+similar+to+Excel+VBA+Range.FormulaLocal
[6]: https://docs.aspose.com/display/cellsnet/Prefix+Table+Elements+Styles+with+HtmlSaveOptions.TableCssId+property
[7]: https://docs.aspose.com/display/cellsnet/Render+Office+Add-Ins+while+converting+Excel+to+Pdf
[8]: https://docs.aspose.com/display/cellsnet/Set+the+Shape+Type+of+Data+Labels+of+Chart
[9]: https://docs.aspose.com/display/cellsnet/Text+overflows+from+GridDesktop+cell+if+it+is+too+long
[10]: https://docs.aspose.com/display/cellsnet/Update+Days+Preserving+History+of+Revision+Logs+in+Shared+Workbook
[11]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[12]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[13]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[14]: https://products.aspose.com/cells/net
[15]: https://downloads.aspose.com/cells/net
[16]: https://docs.aspose.com/display/cellsnet/home
[17]: https://apireference.aspose.com/
[18]: https://forum.aspose.com/c/cells
[19]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




