---
title: 'Strategize the Calculation Precision, Copy Row Heights While Copying Ranges, Size is Reduced and Many More in Aspose.Cells for Android 8.5.0'
date: Tue, 07 Jul 2015 10:03:17 +0000
draft: false
url: /2015/07/07/strategize-the-calculation-precision-copy-row-heights-while-copying-ranges-size-is-reduced-and-many-more-in-aspose.cells-for-android-8.5.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Android logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png)Aspose.Cells for Android 8.5.0 has been released. This release contains many useful features and improvements. Below, we list some major features and other enhancements in the new release.

## Reduced Size of Aspose.Cells for Android

Aspose.Cells uses some third party libraries. For example, there is one thrid-party library which Aspose.Cells uses: bcprov-jdk15-146.jar ([http://www.bouncycastle.org/java.html][2] that is used for AES encryption supported by MS Excel 2010. Sometimes, when using multiple components in an Android project, you might encounter "Unable to execute DX" error which means the total number of methods in the project should not exceed 65536. Now we put the third party lib(s) to an APK (aspose-cells-x.x.x-libs.apk) file. This way, the methods in the third party lib are not needed to be counted any more. Now we only have our Aspose.Cells lib so, the long list of third party library methods are reduced as these run in the same process of the component's main jar.

## Strategize the Calculation Precision

Aspose.Cells for Android 8.5.0 has exposed the CalculationOptions class, CalculationPrecisionStrategy enumeration and a set of new CalculateFormula methods in order to add more flexibility & extensibility to the formula calculation engine. These new APIs were added to facilitate the user who wish to strategize the calculation precision handling on their own according to the application requirements. Please note, due to the precision issue of IEEE 754 Floating-Point Arithmetic, some seemingly simple formulas may not give expected results therefore the latest API build has exposed the following CalculationPrecisionStrategy fields to get desired results according to the selection.

*   CalculationPrecisionStrategy.DECIMAL: Uses decimal as operand where possible, and is most inefficient mode from performance perspective.
*   CalculationPrecisionStrategy.ROUND: Rounds the calculation results according to significant digit.
*   CalculationPrecisionStrategy.NONE: No strategy is applied therefore during the calculation the engine uses the original double value as operand and return the result directly. This option is most efficient and is applicable for most cases.

Aspose.Cells for Android 8.5.0 has exposed the CalculationOptions class that has the following properties.

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

Please see the document that explains the usage of PasteType.ROW\_HEIGHTS enumeration field to copy the row heights of source range to the destination range.

## Calculate Page Setup Scaling Factor

Microsoft Excel calculates the page setup scaling factor while using the "Fit to n page(s) wide by m tall" option. Aspose.Cells for Android 8.5.0 has exposed the SheetRender.PageScale property to mimic the aforesaid feature of Excel application. This property returns a double value which can be converted to percentage for scaling notation.

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

## Other Enhancements & Fixes

Since the code base of Aspose.Cells for Android matches the code of relevant .NET and Java versions, so most of the changes, enhancements and fixes are also included in the release.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.5.0, please visit the [download page][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png "Aspose.Cells for Android logo"
[2]: http://www.bouncycastle.org/java.html)
[3]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry638295.aspx




