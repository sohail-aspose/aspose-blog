---
title: 'C++ Spreadsheet Library - Create, Manipulate and Convert Spreadsheets in C++'
date: Wed, 23 Nov 2016 15:57:53 +0000
draft: false
url: /2016/11/23/create-edit-and-convert-excel-spreadsheets-in-cpp/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp-100x100.png" alt="Aspose.Cells for C++">}}


Here at Aspose we work hard to make developers’ lives easier by providing easy-to-use, yet powerful APIs for managing documents of different formats. Aspose.Cells for C++ is one such project; that allows the developers to dynamically create, manipulate and convert spreadsheets without requiring Office Automation or Microsoft Excel application. [Aspose.Cells for C++ 16.11.0][1] is a native C++ library which is now available for public use.

While you are downloading the API build to give it a try, here is a list of supported features along with a few code snippets for quick testing.

## Load & Save Spreadsheets

The first release of Aspose.Cells for C++ supports loading and saving Excel 97-2003 Workbook format (XLS) & Open Office XML format (XLSX) from file path as well as stream. Aspose.Cells for C++ has provided the Workbook class which represents a Microsoft Excel spreadsheet, and provides the properties and methods necessary to work with spreadsheet files. In order to load an existing spreadsheet to an instance of Workbook class, one needs to pass the file path (or stream) to Workbook constructor whereas the Workbook.Save method can be used either for saving the resultant spreadsheet or for conversion. The Save method has many overloads that can be used to save files in different ways such as on disc or in stream. One of the said overloads accepts an entry from SaveFormat enumeration in order to decide the format for the resultant document.

## Worksheet Manipulation

In order to access the worksheets from a spreadsheet, the Aspose.Cells for C++ has exposed the WorksheetCollection & Worksheet classes. These classes can be used for a multitude of features whereas a few are listed as follow.

*   Add & remove worksheets.
*   Copy & move worksheets.
*   Manage the page breaks.
*   Manage worksheet views.

## Cell Manipulation

A cell is the basic unit of a spreadsheet which can contain data or a formula along with formatting such as font and cell shading. In perspective of Aspose.Cells for C++, a cell is represented by an instance of Cell class whereas a collection of cells is represented by an instance of CellsCollection class. These classes offer a number of features as listed below.

*   Access a particular cell or a range covering all visible cells.
*   Add or retrieve data from a cell.
*   Format a cell or range of cells.
*   Find data or formula.
*   Trace precedent and dependent cells.
*   Create subtotals.

## Row & Column Manipulation

The Aspose.Cells for C++ offers Row & RowCollection classes in order to deal with the worksheet rows whereas Column & ColumnCollection classes have been made available to deal with columns in a worksheet. These classes provide a number of properties and methods in order to manipulate rows and columns as per application requirements. A few of such features are listed as follow.

*   Copy rows & columns
*   Adjust height of rows & width of columns
*   Group/un-group rows & columns
*   Insert/delete rows & columns

## Manage Excel Tables

An Excel table is a matrix of cells containing any number of rows and columns whereas the same table is referred to be as a List Object in Aspose.Cells for C++ APIs. The Aspose::Cells::Tables namespace contains all the necessary classes that deals with the operations related to the List Objects. Most worth mentioning classes are ListObject and ListObjectCollection which allow to create and format List Objects and so on.

## Formula Calculation Engine

Aspose.Cells for C++ has one of its kind custom built formula calculation engine which supports almost all English based Excel functions including text, logical, information, date & time, lookup & reference, math & trigonometry, statistical, database, financial formulas. Aspose.Cells for C++ also provides the ability to insert a function to a cell as well as retrieve the calculated value. The following code snippet demonstrates how simple is to use Aspose.Cells for C++ API to insert a formula and get the calculated value.

```
//Create a new workbook
intrusive_ptr<IWorkbook> wb = Factory::CreateIWorkbook();

//Get first worksheet which is created by default
intrusive_ptr<IWorksheet> ws = wb->GetIWorksheets()->GetObjectByIndex(0);

//Adding a value to "A1" cell
intrusive_ptr<ICell> cell = ws->GetICells()->GetObjectByIndex(new String("A1"));
cell->PutValue(5);

//Adding a value to "A2" cell
cell = ws->GetICells()->GetObjectByIndex(new String("A2"));
cell->PutValue(15);

//Adding a value to "A3" cell
cell = ws->GetICells()->GetObjectByIndex(new String("A3"));
cell->PutValue(25);

//Adding SUM formula to "A4" cell
cell = ws->GetICells()->GetObjectByIndex(new String("A4"));
cell-> SetFormula(new String("=SUM(A1:A3)"));

//Calculating the results of formulas
wb->CalculateFormula();

//Get the calculated value of the cell "A4" and print it on console
cell = ws->GetICells()->GetObjectByIndex(new String("A4"));
printf("Calculated Value of Cell A4: %s\r\n", cell->GetStringValue()->charValue());
```

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][2].
*   [Aspose.Cells for C++ Download Section][3].
*   Aspose.Cells for C++ Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][4] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][5] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: http://downloads.aspose.com/cells/cpp/new-releases/aspose.cells-for-c---16.11.0/
[2]: http://www.aspose.com/products/cells/cpp
[3]: http://downloads.aspose.com/cells/cpp
[4]: https://forum.aspose.com/
[5]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/




