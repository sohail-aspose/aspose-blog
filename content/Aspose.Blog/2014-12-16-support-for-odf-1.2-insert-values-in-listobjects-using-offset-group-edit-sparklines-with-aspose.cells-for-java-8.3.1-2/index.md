---
title: 'Support for ODF 1.2, Insert Values in ListObjects using Offset, Copy Sparkline Group with Aspose.Cells for Java 8.3.1'
date: Tue, 16 Dec 2014 13:42:32 +0000
draft: false
url: /2014/12/16/support-for-odf-1.2-insert-values-in-listobjects-using-offset-group-edit-sparklines-with-aspose.cells-for-java-8.3.1-2/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")We are pleased to announce that the Aspose.Cells for Java 8.3.1 is now available for public use. This release contains many useful improvements, including the long awaited  support for the ODF 1.2 specifications. Please refer to the release notes of [Aspose.Cells for Java 8.3.1][2] for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section first.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Save ODS File in ODF 1.1 and 1.2 Specifications

Aspose.Cells APIs have extended its support for the OpenDocument Format. Now users can save the ODS (OpenDocument Spreadsheets) in conformance to ODF 1.2 specifications. Aspose.Cells APIs have exposed the methods isStrictSchema11 & setStrictSchema11 for the OdsSaveOptions class to support this feature. The default value of the setStrictSchema11 property is false, which means that from version 8.3.1 of Aspose.Cells, ODS files will be saved as ODF format version 1.2 by default. For more details, please check the article Save ODS file in ODF 1.1 and 1.2 Specifications.

## Insert Values in ListObjects using Row/Column Offset

Normally, you add values inside the ListObject/Table using the Cell.putValue method, however, the putValue method must be associated with an instance of a Cell to identify the correct location where value has to be inserted. This mechanism is not usable when you need to add values inside the ListObject using the row and column offsets. Aspose.Cells for Java 8.3.1 has exposed the methods Cell.getTable & ListObject.putCellValue methods to facilitate the users in Accessing the ListObject from a Cell and Add Values using the Row and Column Offsets.

The following sample code loads the source spreadsheet, and adds values inside the table.

```
//Create workbook from source Excel file
Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access cell D5 which lies inside the table
Cell cell = worksheet.getCells().get("D5");

//Put value inside the cell D5
cell.putValue("D5 Data");

//Access the Table from this cell
ListObject table = cell.getTable();

//Add some value using Row and Column Offset
table.putCellValue(2, 2, "Offset [2,2]");

//Save the workbook
workbook.save("output.xlsx"); 
```

## Create Sparkline by Specifying Data Range and Location

Aspose.Cells APIs have exposed the SparklineCollection.add(String dataRange, int row, int column) method to Specify the Data Range and Location of Sparkline Group. Please note, Excel provides the same feature through following steps.

1.  Select the cell containing your Sparkline.
2.  Select Edit Data from the Sparkline section inside the Design tab.
3.  Choose Edit Group Location & Data.
4.  Specify Data Range & Location.

You may achieve the same as discussed above while using the following code snippet.

```
//Create workbook from source Excel file
Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access the first sparkline group
SparklineGroup group = worksheet.getSparklineGroupCollection().get(0);

//Add Data Ranges and Locations inside this sparkline group
group.getSparklineCollection().add("D5:O5", 4, 15);
group.getSparklineCollection().add("D6:O6", 5, 15);
group.getSparklineCollection().add("D7:O7", 6, 15);
group.getSparklineCollection().add("D8:O8", 7, 15);

//Save the workbook
workbook.save("output.xlsx"); 
```

## Other Enhancements & Improvements

The most notable  enhancements in this release are as follow:

*   Improved the Sparkline rendering.
*   Improved the Chart rendering mechanism to address the misalignment of legend entries.
*   Tweaked the rendering engine to generate PDF that are now much closer to how Excel does.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry592876.aspx "Download Aspose.Cells for Java 8.3.1"
[3]: https://forum.aspose.com/




