---
title: 'Strategize the Calculation Precision and Use PageSetup Scaling Factor in Spreadsheets'
date: Mon, 29 Jun 2015 11:36:11 +0000
draft: false
url: /2015/06/29/strategize-calculation-precision-in-excel/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce that Aspose.Cells for Java 8.5.0 is now available for public use. This release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.5.0][1] for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Strategize the Calculation Precision

Aspose.Cells for Java 8.5.0 has exposed the CalculationOptions class, CalculationPrecisionStrategy enumeration and a set of new CalculateFormula methods in order to add more flexibility & extensibility to the formula calculation engine. These new APIs were added to facilitate the user who wish to strategize the calculation precision handling on their own according to the application requirements. Please note, due to the precision issue of IEEE 754 Floating-Point Arithmetic, some seemingly simple formulas may not give expected results therefore the latest API build has exposed the following CalculationPrecisionStrategy fields to get desired results according to the selection.

*   CalculationPrecisionStrategy.DECIMAL: Uses decimal as operand where possible, and is most inefficient mode from performance perspective.
*   CalculationPrecisionStrategy.ROUND: Rounds the calculation results according to significant digit.
*   CalculationPrecisionStrategy.NONE: No strategy is applied therefore during the calculation the engine uses the original double value as operand and return the result directly. This option is most efficient and is applicable for most cases.

Aspose.Cells for Java 8.5.0 has exposed the CalculationOptions class that has the following properties.

*   CalculationOptions.CalcStackSize: Specifies the stack size for calculating cells recursively. -1 specifies that the calculation will use the WorkbookSettings.CalcStackSize of corresponding Workbook.
*   CalculationOptions.CustomFunction: Extends the formula calculation engine with custom formula.
*   CalculationOptions.IgnoreError: Boolean type value indicates if errors are to be hidden while calculating the formulas, where the errors could be due to the unsupported function, external link or more.
*   CalculationOptions.PrecisionStrategy: Accepts a parameter of CalculationPrecisionStrategy type that specifies the strategy for processing precision of calculation.

The CalculationOptions class can now be used with the following methods.

*   Workbook.calculateFormula(CalculationOptions options)
*   Worksheet.calculateFormula(CalculationOptions options, bool recursive)
*   Cell.calculate(CalculationOptions options)

## Copy Row Heights While Copying Ranges

Aspose.Cells APIs have exposed the PasteType.ROW\_HEIGHTS enumeration field for the purpose of copying the row heights while copying the ranges. Upon setting the PasteOptions.PasteType property to PasteType.ROW\_HEIGHTS the heights of all the rows inside the source range will be copied to the destination range.

The following sample code explains the usage of PasteType.ROW\_HEIGHTS enumeration field to copy the row heights of source range to the destination range.

```
//Create workbook object
Workbook workbook = new Workbook();

//Source worksheet
Worksheet srcSheet = workbook.getWorksheets().get(0);

//Add destination worksheet
Worksheet dstSheet = workbook.getWorksheets().add("Destination Sheet");

//Set the row height of the 4th row
//This row height will be copied to destination range
srcSheet.getCells().setRowHeight(3, 50);

//Create source range to be copied
Range srcRange = srcSheet.getCells().createRange("A1:D10");

//Create destination range in destination worksheet
Range dstRange = dstSheet.getCells().createRange("A1:D10");

//Create an instance of PasteOptions
//Set PasteType to PasteType.ROW_HEIGHTS
PasteOptions opts = new PasteOptions();
opts.setPasteType(PasteType.ROW_HEIGHTS);

//Copy source range to destination range while passing the instance of PasteOptions
dstRange.copy(srcRange, opts);

//Write informative message in cell D4 of destination worksheet
dstSheet.getCells().get("D4").putValue("Row heights of source range copied to destination range");

//Save the workbook in XLSX format
workbook.save("output.xlsx", SaveFormat.XLSX);
```

## Calculate Page Setup Scaling Factor

Microsoft Excel calculates the page setup scaling factor while using the "Fit to n page(s) wide by m tall" option. Aspose.Cells for Java 8.5.0 has exposed the SheetRender.PageScale property to mimic the aforesaid feature of Excel application. This property returns a double value which can be converted to percentage for scaling notation.

The following sample code illustrates how to calculate page setup scaling factor using SheetRender.PageScale property.

```
//Create workbook object
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Put some data in these cells
worksheet.getCells().get("A4").putValue("Test");
worksheet.getCells().get("S4").putValue("Test");

//Set paper size
worksheet.getPageSetup().setPaperSize(PaperSizeType.PAPER_A_4);

//Set fit to pages wide as 1
worksheet.getPageSetup().setFitToPagesWide(1);

//Calculate page scale via sheet render
SheetRender sr = new SheetRender(worksheet, new ImageOrPrintOptions());

//Write the page scale value
System.out.println(sr.getPageScale());
```

## Get Cell String Value With or Without Formatting

With this revision, the API has exposed the Cell.getStringValue method along with an enumeration CellValueFormatStrategy that can be used to extract the cell value with or without formatting applied. The newly exposed Cell.getStringValue() method can be used to get the string value of the cell with or without any formatting.

Suppose, you have a cell with value 0.012345 and you have formatted it to display two decimal places only. It will then display as 0.01 in Excel. You can retrieve string values both as 0.01 and as 0.012345 using the Cell.getStringValue() method.

## Other Enhancements & Improvements

The most notable  enhancements in this release are as follow:

*   Improved the HTML rendering and handled a few JavaScript errors.
*   Improved the PDF rendering for Hebrew characters, wrapped text, page break handling & Right to Left rendering.
*   Tweaked calculate engine for handling custom functions.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][2].




[1]: https://products.aspose.com/cells/java
[2]: https://forum.aspose.com/




