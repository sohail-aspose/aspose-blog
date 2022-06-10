---
title: 'Java: Create Signature Line and Specify Absolute PivotItem Position in Excel Files'
date: Tue, 27 Jan 2015 15:24:32 +0000
draft: false
url: /2015/01/27/java-create-signature-line-in-spreadsheets/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


[Aspose.Cell for Java][1] 8.3.2 has been released and we are pleased to announce that this month’s release contains many useful improvements and features. Most worth mentioning feature is the support for Signature Line. Please refer to the release notes of [Aspose.Cells for Java 8.3.2][2] for a full list of bug fixes and improvements along with details on what has been changed in the public API since the previous release. If you are planning to upgrade the Aspose.Cells for Java API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API since your current version.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Support for Signature Line

Microsoft Excel provides the feature to add Signature Line in Excel spreadsheets by clicking the Insert tab and then selecting the Signature Line from the Text group. This feature allows adding the information about the person whose signatures are required on the document while supplying some key information such as name, designation, email address and so on. Aspose.Cells also provides this feature and has exposed the Picture.setSignatureLine field and SignatureLine class for this purpose. For more details, please go through the detailed article on Creating Signature Line in a Spreadsheet.

## Specify Absolute PivotItem Position

Another worth mentioning feature is the support for Absolute Positioning of the PivotItem. Aspose.Cells for Java 8.3.2 has provided this support by exposing a series of new fields that can be used to specify the position of a PivotItem within a parent node and also in the complete collection.

Here are a few details about the newly exposed fields whereas the code snippets are available in the detailed article as linked above.

*   PivotItem.setPosition field can be used to specify the position index in the PivotItemCollection regardless of the parent node.
*   PivotItem.move(int count, boolean isSameParent) method can be used to move the item up or down based on the count value, where count is the number of position to move the PivotItem up or down. If the count value is less than zero, the item will move up in the hierarchy where as if the count value is larger than zero, the PivotItem will move down. The Boolean type isSameParent parameter specify whether the moving operation has to be performed in the same parent node or not.
*   PivotItem.setPositionInSameParentNode field that can be used to specify the position index in the PivotItemCollection under the same parent node.

Important point to note here is that before using any of the above mentioned fields/methods it is necessary to call the PivotTable.refreshData and PivotTable.calculateData methods first.

## Support for Custom Number Decimal and Group Separators

While using Microsoft Excel application, the user can specify the custom Decimal and Thousands separators instead of using the system's predefined separators for a particular spreadsheet. Same can be achieved using the Aspose.Cells for Java API by using the newly exposed fields such as setNumberDecimalSeparator and setNumberGroupSeparator for the WorkbookSettings class. Please check the detailed article on Specify Custom Decimal & Group Separators.

## Improved Worksheet & Workbook Printing

Aspose.Cells for Java 8.3.2 has exposed two new overloads for the SheetRender.toPrinter & same for the WorkbookRender.toPrinter. One of the new overloads accept two integer parameters along with a string parameter for the printer name and prints a range of Worksheet & Workbook pages to the printer. Other overload accepts a string parameter to specify the printing job name along with the printer name.

Signatures of the above discussed overloads are as follow.

*   WorkbookRender.toPrinter(String printerName, int printPageIndex, int printPageCount)
*   SheetRender.toPrinter(String printerName, int printPageIndex, int printPageCount)
*   WorkbookRender.toPrinter(String printerName, String jobName)
*   SheetRender.toPrinter(String printerName, String jobName)

## Enable the Rendering of Unsupported Unicode Characters

Some Unicode characters cannot be displayed using any specified font but they can be displayed with another font family. One of such Unicode character is the Non-breaking Hyphen (U+2011) and its Unicode number is 8209. This character cannot be displayed with Times New Roman but it can be displayed with other fonts like Arial Unicode MS.

When a spreadsheet containing such characters is to rendered on PDF canvas while using a not supporting font family like Times New Roman, the Aspose.Cells API used to change the font of entire word or sentence to another font which could display this character. However, this could be an undesirable behavior for some users and they want only that specific character's font to be changed instead of changing the font of entire word or sentence. In order to deal with this scenario, the Aspose.Cells for Java 8.3.2 API has exposed the setFontSubstitutionCharGranularity field for the PdfSaveOptions class which should be set to true so that only the font of specific character to be changed to another displayable font whereas the rest of the word or sentence should remain in original font.

## Determine which Axis exists in a Chart

Charts can be of any type, where a few chart types such as all the variations of the Pie and Doughnut does not have any axis. Previously, it was not possible to retrieve the information about the particular axis of a given chart but with the release of Aspose.Cells for Java 8.3.2, the API has exposed the Chart.hasAxis method to determine if the chart has a particular axis or not.

You may achieve the same as discussed above while using the following code snippet.

```
 //Create workbook object from source
Workbook workbook = new Workbook("source.xlsx");

//Access the worksheet containing the desired chart
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access the desired chart from the collection
Chart chart = worksheet.getCharts().get(0);

//Determine which axis exists in the chart
boolean ret = chart.hasAxis(AxisType.CATEGORY, true);
System.out.println("Has Primary Category Axis: " + ret);

ret = chart.hasAxis(AxisType.CATEGORY, false);
System.out.println("Has Secondary Category Axis: " + ret);

ret = chart.hasAxis(AxisType.VALUE, true);
System.out.println("Has Primary Value Axis: " + ret);

ret = chart.hasAxis(AxisType.VALUE, false);
System.out.println("Has Seconary Value Axis: " + ret); 
```

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][3].




[1]: https://products.aspose.com/cells/java
[2]: https://downloads.aspose.com/cells/java
[3]: https://forum.aspose.com/




