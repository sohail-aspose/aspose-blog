---
title: 'Copy Row Heights and Calculate Page Setup Scaling Factor in Excel using C#'
date: Mon, 29 Jun 2015 08:51:03 +0000
draft: false
url: /2015/06/29/c-copy-row-heights-and-calculate-page-setup-scaling-factor-in-excel/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


[Aspose.Cells for .NET][1] 8.5.0 has been released. This release contains some useful features and other enhancements. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Determine if the License is Loaded Successfully

Aspose.Cells provides Workbook.IsLicensed property which you can use to determine if the license is loaded successfully or not. If you access this property before setting the license, it will return false and if you will call this property after setting the license, it will return true indicating that license has been loaded successfully. Please see the document on how to determine if the license is loaded successfully or not.

## Strategize the Calculation Precision

Aspose.Cells for .NET 8.5.0 has exposed the CalculationOptions class, CalculationPrecisionStrategy enumeration and a set of new CalculateFormula methods in order to add more flexibility & extensibility to the formula calculation engine. These new APIs were added to facilitate the user who wish to strategize the calculation precision handling on their own according to the application requirements. Please note, due to the precision issue of IEEE 754 Floating-Point Arithmetic, some seemingly simple formulas may not give expected results therefore the latest API build has exposed the following CalculationPrecisionStrategy fields to get desired results according to the selection.

*   CalculationPrecisionStrategy.Decimal: Uses decimal as operand where possible, and is most inefficient mode from performance perspective.
*   CalculationPrecisionStrategy.Round: Rounds the calculation results according to significant digit.
*   CalculationPrecisionStrategy.None: No strategy is applied therefore during the calculation the engine uses the original double value as operand and return the result directly. This option is most efficient and is applicable for most cases.

Aspose.Cells for .NET 8.5.0 has exposed the CalculationOptions class that has the following properties.

*   CalculationOptions.CalcStackSize: Specifies the stack size for calculating cells recursively. -1 specifies that the calculation will use the WorkbookSettings.CalcStackSize of corresponding Workbook.
*   CalculationOptions.CustomFunction: Extends the formula calculation engine with custom formula.
*   CalculationOptions.IgnoreError: Boolean type value indicates if errors are to be hidden while calculating the formulas, where the errors could be due to the unsupported function, external link or more.
*   CalculationOptions.PrecisionStrategy: Accepts a parameter of CalculationPrecisionStrategy type that specifies the strategy for processing precision of calculation.

The CalculationOptions class can now be used with following CalculateFormula methods.

*   Workbook.CalculateFormula(CalculationOptions options)
*   Worksheet.CalculateFormula(CalculationOptions options, bool recursive)
*   Cell.Calculate(CalculationOptions options)

## Copy Row Heights While Copying Ranges

Aspose.Cells APIs have exposed the PasteType.RowHeights enumeration field for the purpose of copying the row heights while copying the ranges. Upon setting the PasteOptions.PasteType property to PasteType.RowHeights the heights of all the rows inside the source range will be copied to destination range.

The following sample code explains the usage of PasteType.RowHeights enumeration field to copy the row heights of source range to the destination range.

```
//Create workbook object
Workbook workbook = new Workbook();

//Source worksheet
Worksheet srcSheet = workbook.Worksheets[0];

//Add destination worksheet
Worksheet dstSheet = workbook.Worksheets.Add("Destination Sheet");

//Set the row height of the 4th row
//This row height will be copied to destination range
srcSheet.Cells.SetRowHeight(3, 50);

//Create source range to be copied
Range srcRange = srcSheet.Cells.CreateRange("A1:D10");

//Create destination range in destination worksheet
Range dstRange = dstSheet.Cells.CreateRange("A1:D10");

//PasteOptions, we want to copy row heights of source range to destination range
PasteOptions opts = new PasteOptions();
opts.PasteType = PasteType.RowHeights;

//Copy source range to destination range with paste options
dstRange.Copy(srcRange, opts);

//Write informative message in cell D4 of destination worksheet
dstSheet.Cells["D4"].PutValue("Row heights of source range copied to destination range");

//Save the workbook in xlsx format
workbook.Save("output.xlsx", SaveFormat.Xlsx);
```

## Calculate Page Setup Scaling Factor

Microsoft Excel calculates the page setup scaling factor while using the "Fit to n page(s) wide by m tall" option. Aspose.Cells for .NET 8.5.0 has exposed the SheetRender.PageScale property to mimic the aforesaid feature of Excel application. This property returns a double value which can be converted to a percentage for scaling notation.

The following sample code illustrates how to calculate page setup scaling factor using SheetRender.PageScale property.

```
//Create workbook object
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Put some data in these cells
worksheet.Cells["A4"].PutValue("Test");
worksheet.Cells["S4"].PutValue("Test");

//Set paper size
worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;

//Set fit to pages wide as 1
worksheet.PageSetup.FitToPagesWide = 1;

//Calculate page scale via sheet render
SheetRender sr = new SheetRender(worksheet, new ImageOrPrintOptions());

//Convert page scale double value to percentage
string strPageScale = sr.PageScale.ToString("0%");

//Write the page scale value
Console.WriteLine(strPageScale);
```

## Get Cell String Value With or Without Formatting

With this revision, the API has exposed the Cell.GetStringValue method along with an enumeration CellValueFormatStrategy that can be used to extract the cell value with and without formatting applied. The newly exposed Cell.GetStringValue() method can be used to get the string value of the cell with or without any formatting.

Suppose, you have a cell with value 0.012345 and you have formatted it to display two decimal places only. It will then display as 0.01 in Excel. You can retrieve string values both as 0.01 and as 0.012345 using the Cell.GetStringValue() method.

## Other Enhancements and Fixes

In the new version, we have also provided the following new features/ enhancements:

*   Provided support to convert Revision of XLSB to XLSM.
*   Render Custom Date Format Pattern g and ge mm dd.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, manipulating Pivot Tables, applying conditional formatting, manipulating drawing objects and shapes, rendering images from Excel worksheets, manipulating charts with formatting, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have also enhanced the Aspose.Cells formula calculation engine and fixed a few issues in this regard.

We have also supported to zoom in or out on the worksheet in the desktop based Grid control by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.5.0, please visit the [download page][2].




[1]: https://products.aspose.com/cells/net
[2]: https://downloads.aspose.com/cells/java




