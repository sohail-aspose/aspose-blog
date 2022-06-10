---
title: 'Get Data Validation Rules Applied to Cells in Excel using C#'
date: Tue, 23 Sep 2014 14:54:58 +0000
draft: false
url: /2014/09/23/get-cell-data-validation-rules-in-excel-verify-cell-validation-rules-csharp-asp.net/
author: Babar Raza
summary: ''
tags: ['Absolute Position', 'Babar Raza', 'Cell Validation', 'Data Validation', 'Excel API', 'Spreadsheet Creation', 'Spreadsheet Manipulation', 'Worksheet', 'shapes']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We have just released this month’s improvements to Aspose.Cells for .NET by upgrading the API to version 8.2.1. This release contains 30 improvements, including the features showcased below. You can download the latest Aspose.Cells for .NET release from the [download section][1] now, and start exploring the new features.

## Get Data Validation Rules of a Cell in Excel

Aspose.Cells for .NET is an easy to use spreadsheet creation, manipulation, and conversion API that provides all the features that Microsoft Excel provides. Cell validation is one of the features that spreadsheet designers use to stop users from inserting invalid values into a particular cell. With the release of Aspose.Cells for .NET 8.2.1, the API has exposed a simple mechanism that identifies if data validation has been applied on a cell. Use the Cell.GetValidation method to acquire any applied validation. If there is no validation, the method returns null. Similarly, use Validations.GetValidationInCell method to acquire the validation applied on any cell by providing its row and column indices.

The following code sample shows how to get validation applied to a cell in Excel using C#.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingRowsColumnsCells-GetValidationAppliedOnCell-GetValidationAppliedOnCell.cs" >}}

Read more about [cell validation][2].

## Verification of Cell Data Validation Rules in Excel

In addition to determining whether validation has been applied, you can also verify if a given value satisfies the data validation rules for a particular cell. This feature is useful in scenarios when you want to [verify if the value entered in the cell satisfies the data validation rules on the fly][3]. The Aspose.Cells API has exposed the GetValidationValue method for the Cell class. If the value entered in a cell does not satisfy the data validation rules, the Cell.GetValidationValue method returns false. The following code sample shows how to verify the data validation rules in C#.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-DataValidationRules-1.cs" >}}

## Find the Absolute Position of Shape in Worksheet

Prior to the release of Aspose.Cells for .NET 8.2.1, it was not easy to calculate the absolute position of a given shape in a worksheet. The latest revision of Aspose.Cells for .NET has exposed a simple mechanism for achieving this by exposing the LeftToCorner and TopToCorner properties for the Shape class. These properties store the absolute position of the shape inside the worksheet in the unit of pixels. The following code sample shows how to find the absolute position of shapes in an Excel worksheet.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManageChartsAndShapes-AbsolutePositionOfShapeInsideWorksheet-1.cs" >}}

Please read more about [finding the absolute position of shape in a worksheet][4].

## Other Enhancements and Fixes

We have fixed a number of critical issues with this release. The most noteworthy problems that version 8.2.1 has fixed are listed below.

*   Fixed a few problems that caused the System.ArgumentException & System.IndexOutOfRangeException.
*   Improved the features related to the hyperlinks in a spreadsheet.
*   Enhanced the PDF rendering engine to improve the fidelity of rendered shapes, charts & page breaks.

Please visit the [documentation][5] for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][6].




[1]: https://downloads.aspose.com/cells/net
[2]: https://docs.aspose.com/display/cellsnet/Get+Validation+applied+on+a+Cell
[3]: https://docs.aspose.com/display/cellsnet/Verify+that+Cell+Value+satisfies+Data+Validation+Rules
[4]: https://docs.aspose.com/display/cellsnet/Finding+Absolute+Position+of+Shape+inside+the+Worksheet
[5]: http://docs.aspose.com/display/cellsnet/Programmers+Guide
[6]: https://forum.aspose.com/




