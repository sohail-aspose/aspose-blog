---
title: 'Search in Cells Based on Original Values, Access Query Table Properties &amp; Enhancements to Formula Calculation Engine with Aspose.Cells for Java 8.7.1'
date: Wed, 02 Mar 2016 13:38:00 +0000
draft: false
url: /2016/03/02/search-in-cells-based-on-original-values-access-query-table-properties-enhancements-to-formula-calculation-engine-with-aspose.cells-for-java-8.7.1/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")Aspose.Cells for Java API has been upgraded to 8.7.1, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.7.1][2] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Search in Cells Based on Original Values

Aspose.Cells APIs already support the Find or Search Data feature for spreadsheets in order to find some particular piece of contents in cell value & formula. However, this feature was lacking the aspect of formatting applied onto the cell that may change the appearance as well as the value of the cell, consequently making the content unsearchable using the original value. With this release of Aspose.Cells for Java API, another constant by the name LookInType.ORIGINAL\_VALUES has been exposed to the public API which allows to overcome the situation as discussed above.

The following piece of code demonstrates the usage of LookInType.ORIGINAL\_VALUES property to search the cells based on original values.

```
//Create workbook object
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Add 10 to cells A1 and A2
worksheet.getCells().get("A1").putValue(10);
worksheet.getCells().get("A2").putValue(10);

//Add Sum formula to cell D4
Cell cell = worksheet.getCells().get("D4");
cell.setFormula("=Sum(A1:A2)");

//Format the value to show as --- instead of original value
Style style = cell.getStyle();
style.setCustom("---");
cell.setStyle(style);

//Calculate the workbook
workbook.calculateFormula();

//Create find options and search for value 20
FindOptions options = new FindOptions();
options.setLookInType(LookInType.ORIGINAL_VALUES);
options.setLookAtType(LookAtType.ENTIRE_CONTENT);

Cell foundCell = null;
Object obj = 20;

//Find 20 which is Sum(A1:A2) and formatted as ---
foundCell = worksheet.getCells().find(obj, foundCell, options); 
```

## Access Query Table Properties

Aspose.Cells for Java 8.7.1 has exposed the boolean type QueryTable.PreserveFormatting & QueryTable.AdjustColumnWidth properties in order to mimic the Excel's features of preserving cell formatting & adjusting column widths while working with External Data Range of type Query Table.

Please note, Excel application provides these options to influence the formatting of the data where the options can be accessed on Excel interface from **Data** tab by clicking the **Properties** button as shown below.

The following piece of code shows the simple usage scenario of QueryTable.PreserveFormatting &QueryTable.AdjustColumnWidth properties.

```
//Create an instance of Worbook from existing spreadsheet
Workbook workbook = new Workbook(inFilePath);

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access first Query Table from the collection
QueryTable qt = worksheet.getQueryTables().get(0);

//Print Query Table properties
System.out.println("Adjust Column Width: " + qt.getAdjustColumnWidth());
System.out.println("Preserve Formatting: " + qt.getPreserveFormatting());

//Set Preserve Formatting to true
qt.setPreserveFormatting(true);

//Save the workbook
workbook.save(outFilePath); 
```

## Enhancements to Formula Calculation Engine

Aspose.Cells APIs have enhanced the formula calculation engine with this release where the most worth mentioning enhancements are as follow.

### Support for Array Formulas of Data Tables

In perspective of Excel application, Data tables are part of a suite of commands that are called what-if analysis tools. These tools can be used to process the formulas by changing the values in cells to see how those changes will affect the outcome of formulas on the worksheet. With this release of Aspose.Cells for Java, the API now allows you to calculate the array formula of Data Tables. Please note, no new API have been exposed for this feature and all enhancements are done internally to the formula calculation engine therefore by simply calling the Workbook.calculateFormula method, all formulas including the array formulas will be computed automatically.

### Support for FORMULATEXT Function

Aspose.Cells for Java 8.7.1 has provided support for the Excel's FORMULATEXT Function which can be used to get the formula string for any given cell as it is being displayed in the Excel's formula bar.

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Enhanced the image rendering engine for SVG file format.
*   Enhanced Chart2Image module to avoid overlapping of chart objects.
*   Enhanced the HTML rendering engine to handle cases involving missing columns.

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
[2]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry694155.aspx
[3]: http://www.aspose.com/java/excel-component.aspx
[4]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[5]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://github.com/asposecells/Aspose_Cells_Java




