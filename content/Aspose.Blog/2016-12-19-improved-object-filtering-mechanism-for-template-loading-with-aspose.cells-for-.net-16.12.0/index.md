---
title: 'Improved Object Filtering Mechanism for Template Loading with Aspose.Cells for .NET 16.12.0'
date: Mon, 19 Dec 2016 11:24:21 +0000
draft: false
url: /2016/12/19/improved-object-filtering-mechanism-for-template-loading-with-aspose.cells-for-.net-16.12.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v16.12.0][2]. The new release includes some features and other enhancements with critical bug fixes. Please see the release notes in order to know what is new/enhanced and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some valuable features and other enhancements here.

## Improved Object Filtering for Loading Templates

Sometimes, application requirement could be to load just a particular type of objects while loading existing spreadsheets in Aspose.Cells' object model. For instance, you may require to load only the cells along with formulas & formatting or just the document properties. Aspose.Cells APIs now provide a flexible yet comprehensive mechanism to achieve such requirements by exposing the LoadFilter class.

The LoadFilter class along with LoadOptions.LoadFilter property can control the type of data/objects to be loaded while initializing an instance of Workbook from a template file. The constructor of the LoadFilter class can accept constant(s) from the LoadDataFilterOptions enumeration, that specifies the type of objects to be loaded.

The LoadDataFilterOptions enumeration currently has the following constants.

*   LoadDataFilterOptions.All: Loads everything from the template file.
*   LoadDataFilterOptions.CellBlank: Loads the blank cells.
*   LoadDataFilterOptions.CellBool: Loads the cells having value of type Boolean.
*   LoadDataFilterOptions.CellData: Loads all cells data including values, formulas and formatting.
*   LoadDataFilterOptions.CellError: Loads cells whose value is error.
*   LoadDataFilterOptions.CellNumeric: Loads the cells having value of type number/numeric.
*   LoadDataFilterOptions.CellString: Loads the cells having value of type string/text.
*   LoadDataFilterOptions.CellValue: Loads the cells value regardless of the type.
*   LoadDataFilterOptions.Chart: Loads the charts.
*   LoadDataFilterOptions.ConditionalFormatting: Loads conditional formatting rules.
*   LoadDataFilterOptions.DataValidation: Loads data validations.
*   LoadDataFilterOptions.DocumentProperties: Loads document properties.
*   LoadDataFilterOptions.Formula: Load formulas including defined Names.
*   LoadDataFilterOptions.MergedArea: Loads merged cells.
*   LoadDataFilterOptions.None: Loads nothing.
*   LoadDataFilterOptions.PivotTable: Loads Pivot Tables.
*   LoadDataFilterOptions.Settings: Loads settings for workbook and worksheet.
*   LoadDataFilterOptions.Shape: Loads all types of shapes.
*   LoadDataFilterOptions.Style: Loads styles for cell formatting.
*   LoadDataFilterOptions.Table: Loads List Objects/Tables.

Here is a simple snippet to load only the document properties from a template file.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing LoadDataFilterOptions.DocumentProperties to constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.DocumentProperties);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.LoadFilter = filter;

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

Following snippet loads everything from an existing spreadsheet except for the charts.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.All & ~LoadDataFilterOptions.Chart);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.LoadFilter = filter;

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

The code snippet ahead loads only the cell values along with the formulas and formatting.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.CellData);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.LoadFilter = filter;

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

The LoadFilter class also allows to customize the loading process as per the properties of the Worksheet. In order to customize the loading process, one has to override the LoadFilter.StartSheet method. Please note, there are just a few properties that can be used for a given worksheet object in this scenario because most of the data and properties have not been loaded yet. The available Worksheet properties are: Name, Index & VisibilityType.

Following snippet demonstrates how to extend the LoadFilter class and override the StartSheet method in order to choose different loading mechanism as per different worksheets in a given template.

```
//Implement your own custom load filter, it will enable you to filter your individual worksheet
class CustomLoadFilter : Aspose.Cells.LoadFilter
{
    public override void StartSheet(Worksheet sheet)
    {
        if (sheet.Name == "NoCharts")
        {
            //Load everything except charts
            this.m_LoadDataFilterOptions = LoadDataFilterOptions.All&~LoadDataFilterOptions.Chart;
        }

        if (sheet.Name == "NoShapes")
        {
            //Load everything except shapes
            this.m_LoadDataFilterOptions = LoadDataFilterOptions.All & ~LoadDataFilterOptions.Shape;
        }

        if (sheet.Name == "NoConditionalFormatting)")
        {
            //Load everything except conditional formatting
            this.m_LoadDataFilterOptions = LoadDataFilterOptions.All & ~LoadDataFilterOptions.ConditionalFormatting;
        }
    }//End StartSheet method.
}//End CustomLoadFilter class. 
```

The newly created class can be used as follow.

```
//Filter worksheets using custom load filter
LoadOptions ldOpts = new LoadOptions();
ldOpts.LoadFilter = new CustomLoadFilter();

//Load the workbook with above filter
Workbook wb = new Workbook("sample.xlsx", ldOpts); 
```

In order to get more in-depth understanding of the new filtering mechanism, please check the detailed article on Filtering Objects at Load Time.

## Other Enhancements and Fixes

Aspose.Cells for .NET 16.12.0 has enhanced its core for more stability. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Ability to export XML map data to disc.
*   Support for ScaleCrop and LinksUpToDate built-in document properties.
*   Support OTS file format.
*   Expand/Collapse grouped rows/columns (Aspose.Cells.GridWeb).
*   Enhanced Aspose.Cells formula calculation engine.
*   Enhanced PDF rendering engine for font substitution while converting charts to PDF format.
*   Handled a few exceptions, such as ArithmeticException & CellsException.

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel Excel file formats, manipulating and rendering charts and other shapes, manipulating and formatting PivotTables, conditional formatting, copying cells in the worksheet, rendering to HTML file format, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

## Changes to the Public API

This revision of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow whereas details can be viewed from the Migration Manual.

*   The LoadDataOptions, LoadDataFilterOptions, OnlyLoadDocumentProperties & LoadDataAndFormatting properties of the LoadOptions class have been marked obsoleted whereas it is advised to use the LoadOptions.LoadFilter as alternative.
*   The Rotation & Background properties of the DataLabels class have been completely removed from the public API. It is advised to use the DataLabels.RotationAngle & DataLabels.BackgroundModeproperties respectively.
*   The Title.Rotation property has been removed. It is advised to use the Title.RotationAngle property instead.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][3].
*   [Aspose.Cells for .NET Download Section][4].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-16.12.0/
[3]: http://www.aspose.com/.net/excel-component.aspx
[4]: http://www.aspose.com/downloads/cells/net
[5]: http://www.aspose.com/api/net/cells
[6]: https://forum.aspose.com/
[7]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




