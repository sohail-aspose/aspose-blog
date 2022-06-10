---
title: 'Import Data from JSON to Excel in Java using Aspose.Cells for Java'
date: Sat, 20 Apr 2019 10:09:03 +0000
draft: false
url: /2019/04/20/import-data-from-json-using-aspose.cells-for-java-19.3/
author: Ahsaniqbal
summary: ''
tags: ['Autofit rows in Excel in Java', 'Convert Excel table to range', 'Convert JSON to Excel in Java', 'Import Data from JSON to Excel', 'Import Data from JSON to Excel in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java.jpg" alt="Import Data from JSON to Excel">}}


Big smiles as I am here to announce the release of the latest version of Aspose.Cells for Java. In this post, I am going to give you a glimpse of all the new exciting features for the best utilization of the API along with the improvements and fixes. Links to the relevant articles and resources will also be available for quick reference. So let us start reviewing what is there in this [release][1].

## JSON to Excel in Java

As you know that JavaScript Object Notation is a common data interchange format which is quite lightweight and can be read by human and machines easily. Now, for example, you get data from some Web API in JSON format and need it to be imported into some Excel file, then Aspose.Cells is there to provide this facility.

JSONUtility class is introduced by Aspose.Cells for this purpose having an ImportData method that not only imports data from JSON to Excel but also performs different conversions and formatting using the JsonLayoutOptions object during the import process. You may try this exciting feature by following the article [Importing Data from JSON][2]. Here is a sample code to import data from JSON to Excel in Java:

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Data-ImportingFromJson-1.java" >}}

You can see that the result is cool as a fully formatted Excel file is created without using any extra code to parse the JSON string from any source like Web API. Isn't it? For example, if you get the following string from Web API, then the output Excel file is shown in the image below:

_\[{"color": "red","value": "#f00"},{"color": "green","value": "#0f0"},{"color": "blue","value": "#00f"},{"color": "cyan","value": "#0ff"},{"color": "magenta","value": "#f0f"},{"color": "yellow","value":"#ff0"},{"color": "black","value": "#000"}\]_



{{< figure align=center src="images/OutputExcel.png" alt="JSON to Excel Java">}}


## Convert Table to Range with Options

Conversion of the table to a range was available earlier. However what if you want to control the formatting of destination range like formatting only the partial output. The good news is that this feature is available now and you don't need to write extra code to format the output range. We have introduced a new class TableToRangeOptions where LastRow property is available to set the last row to which formatting is copied from the source table. Here is the view of a sample table and converted range which is formatted up to row 5.



{{< figure align=center src="images/RangeTest-1024x375.png" alt="Convert Table Range in Excel">}}


Here is a sample code that is used to create the above range.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Tables-ConvertTableToRangeWithOptions-1.java" >}}

For detailed information on conversions follow [this][3] link.

## Get Range with External Links

Microsoft Excel supports external links for fetching data from different sources. We have provided the option to retrieve these links from the Excel file using [Name.GetRefferedAreas][4] method. This method returns [ReferredArea][5] which has many useful properties as follows:

*   [EndColumn][6]: The end column of the area
*   [EndRow][7]: The end row of the area
*   [ExternalFileName][8]: Get the external file name if this is an external reference
*   [IsArea][9]: Indicates whether this is an area
*   [IsExternalLink][10]: Indicates whether this is an external link
*   [SheetName][11]: Indicates which sheet this reference is in
*   [StartColumn][12]: The start column of the area
*   [StartRow][13]: The start row of the area

In the following example, an external file having named range "Names" is linked with the Excel file. We can access this named range in the linked file and display its properties mentioned above.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-GetRangeWithExternalLinks-1.java" >}}

## Keep Separators for Blank Rows in Spreadsheet to CSV

Many times you convert the Excel sheets to CSV for using it in some other environment or applications. You may need to decide yourself about the separators for blank rows in the spreadsheet while exporting it to CSV. For example, there is a blank row in the source spreadsheet and you want either a blank row in the CSV or have a row with predefined separators. We have provided this feature now and you can get details about this feature [here][14].

For better understanding, have a look at the following image which shows the result of this feature.



{{< figure align=center src="images/KeepSeparator.png" alt="Excel to CSV Java">}}


Following is a sample code which demonstrates this new feature.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-KeepSeparatorsForBlankRow-1.java" >}}

## Autofit Rows for Merged Cells

Autofitting rows is a very common operation that you perform while working with the Excel files. This feature was already there in Aspose.Cells API however many people asked for more control over this operation. To fulfill this requirement we have provided [AutoFitMergedCellsType][15] enumerator which contains the following options:

*   [NONE][16]: Ignore merged cells.
*   [FIRST\_LINE][17]: Only expands the height of the first row.
*   [LAST\_LINE][18]: Only expands the height of the last row.
*   [EACH\_LINE][19]: Expands the height of each row.

Here is a snapshot of this feature where the effect of one of the options EACH\_LINE is shown.



{{< figure align=center src="images/Screenshot-2019-04-18-at-2.48.54-PM.png" alt="Autofit Rows in Excel">}}


You can test this feature using following sample code.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-RowsAndColumns-AutofitRowsforMergedCells-1.java" >}}

For more details on this topic please visit [here][20].

## Other enhancements in this release

*   Text extraction from cells using Cell.getDisplayStringValue() was returning different results for Ricty Diminished font. The new version returns an appropriate string now.
*   Text alignment in the resultant PDF is made more accurate.
*   In some cases, the black text color was changed to red in the converted HTML, that is no more an issue.
*   A Scatter chart and 2D bubble chart will be rendered to PDF without any problem.
*   Range.Copy() will copy the font settings and other objects now onward.
*   Workbook.hasExernalLinks() will return proper results for DDE links.

Note: You may download [this][21] project from GitHub to get the template files and running examples used in this blog post.




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.3+Release+Notes
[2]: https://docs.aspose.com/display/cellsjava/Import+and+Export+Data#ImportandExportData-ImportingDatafromJSON
[3]: https://docs.aspose.com/display/cellsjava/Convert+an+Excel+Table+to+a+Range+of+Data#ConvertanExcelTabletoaRangeofData-ConvertTabletoRangewithOptions
[4]: https://apireference.aspose.com/java/cells/com.aspose.cells/name#getReferredAreas(boolean)
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/ReferredArea
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#EndColumn
[7]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#EndRow
[8]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#ExternalFileName
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#IsArea
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#IsExternalLink
[11]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#SheetName
[12]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#StartColumn
[13]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#StartRow
[14]: https://docs.aspose.com/display/cellsjava/Keep+Separators+for+Blank+Rows+while+exporting+spreadsheets+to+CSV+format
[15]: https://apireference.aspose.com/java/cells/com.aspose.cells/AutoFitMergedCellsType
[16]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#NONE
[17]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#FIRST_LINE
[18]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#LAST_LINE
[19]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#EACH_LINE
[20]: https://docs.aspose.com/display/cellsjava/Autofit+Rows+and+Columns#AutofitRowsandColumns-AutoFitRowsforMergedCells
[21]: https://github.com/aspose-cells/Aspose.Cells-for-Java




