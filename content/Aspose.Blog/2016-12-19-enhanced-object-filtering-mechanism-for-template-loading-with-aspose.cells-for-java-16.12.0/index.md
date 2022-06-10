---
title: 'Enhanced Object Filtering Mechanism for Template Loading with Aspose.Cells for Java 16.12.0'
date: Mon, 19 Dec 2016 11:44:44 +0000
draft: false
url: /2016/12/19/enhanced-object-filtering-mechanism-for-template-loading-with-aspose.cells-for-java-16.12.0/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")Aspose team is pleased to announce the release of [Aspose.Cells for Java 16.12.0][2]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Improved Object Filtering for Loading Templates

Sometimes, application requirement could be to load just a particular type of objects while loading existing spreadsheets in Aspose.Cells' object model. For instance, you may require to load only the cells along with formulas & formatting or just the document properties. Aspose.Cells APIs now provide a flexible yet comprehensive mechanism to achieve such requirements by exposing the LoadFilter class.

The LoadFilter class along with LoadOptions.LoadFilter property can control the type of data/objects to be loaded while initializing an instance of Workbook from a template file. The constructor of the LoadFilter class can accept constant(s) from the LoadDataFilterOptions enumeration, that specifies the type of objects to be loaded.

The LoadDataFilterOptions enumeration currently has the following constants.

*   LoadDataFilterOptions.ALL: Loads everything from the template file.
*   LoadDataFilterOptions.CELL\_BLANK: Loads the blank cells.
*   LoadDataFilterOptions.CELL\_BOOL: Loads the cells having value of type Boolean.
*   LoadDataFilterOptions.CELL\_DATA: Loads all cells data including values, formulas and formatting.
*   LoadDataFilterOptions.CELL\_ERROR: Loads cells whose value is error.
*   LoadDataFilterOptions.CELL\_NUMERIC: Loads the cells having value of type number/numeric.
*   LoadDataFilterOptions.CELL\_STRING: Loads the cells having value of type string/text.
*   LoadDataFilterOptions.CELL\_VALUE: Loads cells value regardless of the type.
*   LoadDataFilterOptions.CHART: Loads the charts.
*   LoadDataFilterOptions.CONDITIONAL\_FORMATTING: Loads conditional formatting rules.
*   LoadDataFilterOptions.DATA\_VALIDATION: Loads data validations.
*   LoadDataFilterOptions.DOCUMENT\_PROPERTIES: Loads document properties.
*   LoadDataFilterOptions.FORMULA: Load formulas including defined Names.
*   LoadDataFilterOptions.MERGED\_AREA: Loads merged cells.
*   LoadDataFilterOptions.NONE: Loads nothing.
*   LoadDataFilterOptions.PIVOT\_TABLE: Loads Pivot Tables.
*   LoadDataFilterOptions.SETTINGS: Loads settings for workbook and worksheet.
*   LoadDataFilterOptions.SHAPE: Loads all types of shapes.
*   LoadDataFilterOptions.STYLE: Loads styles for cell formatting.
*   LoadDataFilterOptions.TABLE: Loads List Objects/Tables.

Here is a simple snippet to load only the document properties from a template file.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing LoadDataFilterOptions.DocumentProperties to constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.DOCUMENT_PROPERTIES);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

Following snippet loads everything from an existing spreadsheet except for the charts.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.ALL & ~LoadDataFilterOptions.CHART);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

The code snippet ahead loads only the cell values along with the formulas and formatting.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.CELL_DATA);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

The LoadFilter class also allows to customize the loading process as per the properties of the Worksheet. In order to customize the loading process, one has to override the LoadFilter.startSheet method. Please note, there are just a few properties that can be used for a given worksheet object in this scenario because most of the data and properties have not been loaded yet. The available Worksheet properties are: Name, Index & VisibilityType.

Following snippet demonstrates how to extend the LoadFilter class and override the startSheet method in order to choose different loading mechanism as per worksheets in a given template.

```
public class CustomFilter extends LoadFilter
{
    public void startSheet(Worksheet sheet)
    {
        if (sheet.getName() == "Sheet1")
        {
            //Load everything
            m_LoadDataFilterOptions = LoadDataFilterOptions.ALL;
        }
        else
        {
            //Load nothing
            m_LoadDataFilterOptions = LoadDataFilterOptions.NONE;
        }
    }
} 
```

The newly created class can be used as follow.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Set the LoadFilter property of LoadOptions object to the instance of CustomFilter class created above
options.setLoadFilter(new CustomFilter());

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

In order to get more in-depth understanding of the new filtering mechanism, please check the detailed article on Filtering Objects at Load Time.

## Other Enhancements & Fixes

Aspose.Cells for Java 16.12.0 has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Ability to export XML map data to disc.
*   Support for ScaleCrop and LinksUpToDate built-in document properties.
*   Enhanced PDF rendering engine for font substitution while converting charts to PDF format.
*   Handled a few exceptions such as ArrayIndexOutOfBoundsException & CellsException.

## Changes to the Public API

This revision of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow whereas details can be viewed from the Migration Manual.

*   The LoadDataOptions, LoadDataFilterOptions, OnlyLoadDocumentProperties & LoadDataAndFormatting properties of the LoadOptions class have been marked obsoleted whereas it is advised to use the LoadOptions.LoadFilter as alternative.
*   The Rotation & Background properties of the DataLabels class have been completely removed from the public API. It is advised to use the DataLabels.RotationAngle & DataLabels.BackgroundMode properties respectively.
*   The Title.Rotation property has been removed. It is advised to use the Title.RotationAngle property instead.
*   The Title.getCharacters method has been removed while providing the Title.characters method to achieve the same goal.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][3].
*   [Aspose.Cells for Java Download Section][4].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][7] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][8] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java"
[2]: http://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-16.12.0/ "Download Aspose.Cells for Java 16.12.0"
[3]: http://www.aspose.com/java/excel-component.aspx
[4]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[5]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[8]: https://github.com/asposecells/Aspose_Cells_Java




