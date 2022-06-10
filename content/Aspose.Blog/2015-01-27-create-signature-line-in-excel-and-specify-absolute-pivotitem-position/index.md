---
title: 'Create Signature Line and Specify Absolute PivotItem Position in Excel Files using C#'
date: Tue, 27 Jan 2015 14:25:47 +0000
draft: false
url: /2015/01/27/create-signature-line-in-excel-and-specify-absolute-pivotitem-position/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[Aspose.Cells for .NET][1] 8.3.2 has been released. This release contains some useful features and a number of other enhancements. It contains over 70 fixes and other improvements, including the new features as listed below. The most important new features include support for Signature Line. If you are planning to upgrade the API from a previous release, we suggest you to check documents in the [Public API Changes][2] section.

## Check Password to modify using Aspose.Cells APIs

You can assign _Password to open_ and _Password to modify_ while creating your spreadsheets in Microsoft Excel. This feature is useful when you need to check if the given password matches with the actual Password to modify programmatically. Aspose.Cells provides Workbook.CheckWriteProtectedPassword() method that you can use to [check if the given Password to modify is correct or not][3].

## Support for Signature Line

Microsoft Excel provides the feature to add Signature Line in Excel spreadsheets by clicking the Insert tab and then selecting the Signature Line from the Text group. This feature allows adding the information about the person whose signatures are required on the document while supplying some key information such as name, designation, email address and so on. Aspose.Cells also provides this feature and has exposed the Picture.setSignatureLine field and SignatureLine class for this purpose. For more details, please go through the detailed article on [Creating Signature Line in a Spreadsheet][4].

## Specify Absolute PivotItem Position

Another worth mentioning feature is the support for [Absolute Positioning of the PivotItem][5]. Aspose.Cells for .NET 8.3.2 has provided this support by exposing a series of new attributes that can be used to specify the position of a PivotItem within a parent node and also in the complete collection.

Here are a few details about the newly exposed fields whereas the code snippets are available in the detailed article as linked above.

*   PivotItem.Position property can be used to specify the position index in the PivotItemCollection regardless of the parent node.
*   PivotItem.Move(int count, bool isSameParent) method can be used to move the item up or down based on the count value, where count is the number of position to move the PivotItem up or down. If the count value is less than zero, the item will move up in the hierarchy where as if the count value is larger than zero, the PivotItem will move down. The Boolean type isSameParent parameter specify whether the moving operation has to be performed in the same parent node or not.
*   PivotItem.PositionInSameParentNode property that can be used to specify the position index in the PivotItemCollection under the same parent node.

Important point to note here is that before using any of the above mentioned properties/methods it is necessary to call the PivotTable.RefreshData and PivotTable.CalculateData methods first.

## Support for Custom Number Decimal and Group Separators

While using Microsoft Excel application, the user can specify the custom Decimal and Thousands separators instead of using the system’s predefined separators for a particular spreadsheet. This can be achieved using the Aspose.Cells for .NET API by using the newly exposed attributes such as, NumberDecimalSeparator and NumberGroupSeparator for the WorkbookSettings class. Please check the detailed article on [Specify Custom Decimal & Group Separators][6].

## Improved Worksheet & Workbook Printing

Aspose.Cells for .NET 8.3.2 has exposed two new overloads for the SheetRender.ToPrinter & same for the WorkbookRender.ToPrinter. One of the new overloads accept two integer parameters along with a string parameter for the printer name and prints a range of Worksheet & Workbook pages to the printer. Other overload accepts a string parameter to [specify the printing job name][7] along with the printer name. See the detailed document on [printing range of pages using SheetRender and WorkbookRender][8].

Signatures of the above-discussed overloads are as follow.

*   WorkbookRender.ToPrinter(String printerName, int printPageIndex, int printPageCount)
*   SheetRender.ToPrinter(String printerName, int printPageIndex, int printPageCount)
*   WorkbookRender.ToPrinter(String printerName, String jobName)
*   SheetRender.ToPrinter(String printerName, String jobName)

## Enable the Rendering of Unsupported Unicode Characters

Some Unicode characters cannot be displayed using any specified font but they can be displayed with another font family. One of such Unicode character is the Non-breaking Hyphen (U+2011) and its Unicode number is 8209. This character cannot be displayed with Times New Roman but it can be displayed with other fonts like Arial Unicode MS.

When a spreadsheet containing such characters is rendered on PDF canvas while using a not supporting font family like Times New Roman, the Aspose.Cells API used to change the font of entire word or sentence to another font which could display this character. However, this could be an undesirable behavior for some users and they want only that specific character’s font to be changed instead of changing the font of entire word or sentence. In order to deal with this scenario, the Aspose.Cells for .NET 8.3.2 API has exposed the IsFontSubstitutionCharGranularity property for the PdfSaveOptions class which should be set to true so that only the [font of specific character to be changed to another displayable font][9] whereas the rest of the word or sentence should remain in original font.

## Determine which Axis exists in a Chart

Charts can be of any type, where a few chart types such as all the variations of the Pie and Doughnut does not have any axis. Previously, it was not possible to retrieve the information about the particular axis of a given chart but with the release of Aspose.Cells for .NET 8.3.2, the API has exposed the Chart.HasAxis method to [determine if the chart has a particular axis or not][10].

You may achieve the same as discussed above while using the following code snippet.

```
//Create workbook object
Workbook workbook = new Workbook("source.xlsx");

//Access the first worksheet
Worksheet worksheet = workbook.Worksheets\[0\];

//Access the chart
Chart chart = worksheet.Charts\[0\];

//Determine which axis exists in chart
bool ret = chart.HasAxis(AxisType.Category, true);
Console.WriteLine("Has Primary Category Axis: " + ret);

ret = chart.HasAxis(AxisType.Category, false);
Console.WriteLine("Has Secondary Category Axis: " + ret);

ret = chart.HasAxis(AxisType.Value, true);
Console.WriteLine("Has Primary Value Axis: " + ret);

ret = chart.HasAxis(AxisType.Value, false);
Console.WriteLine("Has Seconary Value Axis: " + ret);

```

## Other Enhancements and Fixes

In the new version, we have also provided the following new enhancements:

*   Render HTML for each sheet with the contents of the element only
*   Aspose.Cells increases the corresponding row height accordingly
*   Render smooth and curved at edges Chart lines
*   Copying a Range with PasteType.All also copies the Hyperlink
*   Enhance exceptions while handling un-supported OOXML file formats

We have fixed a few exceptions that occurred while loading and opening Microsoft Excel file formats. We have also fixed the exceptions that occurred while calculating formulas in the spreadsheets.

We have also supported conditional formatting in the desktop based Grid control provided by Aspose.Cells for .NET. We have added support to create/set named ranges and fixed a few issues in the web based Grid control by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.3.2, please visit the [download page][11].




[1]: https://products.aspose.com/cells/net
[2]: https://docs.aspose.com/cells/net/migrating-from-earlier-versions-of-aspose-cells/
[3]: https://docs.aspose.com/cells/net/check-password-to-modify-using-aspose-cells/
[4]: https://docs.aspose.com/cells/net/create-signature-line-in-an-excel-workbook-using-aspose-cells/
[5]: https://docs.aspose.com/cells/net/specifying-the-absolute-position-of-the-pivot-item/
[6]: https://docs.aspose.com/cells/net/specify-custom-number-decimal-and-group-separators-for-workbook/
[7]: https://docs.aspose.com/cells/net/specify-job-or-document-name-while-printing-with-aspose-cells/
[8]: https://docs.aspose.com/cells/net/printing-range-of-pages-using-sheetrender-and-workbookrender/
[9]: https://docs.aspose.com/cells/net/change-the-font-on-just-the-specific-unicode-characters-while-saving-to-pdf/
[10]: https://docs.aspose.com/cells/net/determine-which-axis-exists-in-the-chart/
[11]: https://downloads.aspose.com/cells/net




