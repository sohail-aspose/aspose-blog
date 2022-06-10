---
title: 'Autofit Rows for Merged Cells using Aspose.Cells for .NET v19.3'
date: Tue, 23 Apr 2019 11:15:38 +0000
draft: false
url: /2019/04/23/autofit-rows-for-merged-cells-using-aspose-cells-for-net-v19-3/
author: Amjad Sahi
summary: ''
tags: ['.NET Excel API', 'Autofit rows in the merged cells Excel', 'Import Data from JSON to Excel']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/products/cells/net "Aspose.Cells for .NET API")Guys, are you ready? Before we dive into its details: I want you to get an essence of the public release. I am giving you little preview of the new features and other enhancements available in the release for quick reference. I guess you know the valuable usage of MS Excel’s auto-fit rows/cols feature. Yet, you are one step ahead and perform the operation on merged cells by Aspose.Cells. While working in MS Excel IDE, you might not dislike formatted Tables but sometimes you need to convert to raw range. Here comes the library to accomplish these tasks via the APIs. Some of you might also like importing from JSON. So let's not wait another moment to review the [release notes][2]. Do you want to know all exciting features and other enhancements? Here you go.

### Autofit Rows for Merged Cells

Autofitting rows is a very common operation which you perform while working with the Excel files. This feature was already there in Aspose.Cells API however many people asked for more control over this operation. To fulfill this requirement we have provided [AutoFitMergedCellsType][3] enumerator which contains the following options:

*   None: Ignore merged cells.
*   FirstLine: Only expands the height of the first row.
*   LastLine: Only expands the height of the last row.
*   EachLine: Expands the height of each row.

Here is a snapshot of this feature where the effect of one of the options EechLine is shown.



{{< figure align=center src="images/Screenshot-2019-04-18-at-2.48.54-PM.png" alt="autofit rows in merged cells in Excel">}}


You can test this feature using following sample code.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-RowsColumns-AutofitRowsforMergedCells-1.cs" >}}

For more details on this topic please visit [here][4].

### Convert Table to Range with Options

Conversion of the table to a range was available earlier. However what if you want to control the formatting of destination range like formatting only the partial output. The good news is that this feature is available now and you don't need to write extra code to format the output range. We have introduced a new class TableToRangeOptions where LastRow property is available to set the last row to which formatting is copied from the source table. Here is the view of a sample table and converted range which is formatted up to row 5.



{{< figure align=center src="images/RangeTest-1024x375.png" alt="Autofit rows in Excel">}}


Here is a sample code which is used to create the above range.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Tables-ConvertTableToRangeWithOptions-1.cs" >}}

For detailed information on conversions follow [this][5] link.

### Import Data from JSON

As you know that JavaScript Object Notation is a common data interchange format which is quite lightweight and can be read by human and machines easily. Now, for example, you get data from some Web API in JSON format and need it to be imported into some Excel file, then Aspose.Cells is there to provide this facility.

JSONUtility class is introduced by Aspose.Cells for this purpose having ImportData method that not only imports data but also performs different conversions and formatting using the JsonLayoutOptions object during the import process. You may try this exciting feature by following article [Importing Data from JSON][6]. Here is a sample code to use this feature:

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Data-Handling-Importing-ImportingFromJson-1.cs" >}}

You can see that result is cool as fully formatted Excel file is created without using any extra code to parse the JSON string from any source like Web API. Isn't it? For example, if you get the following string from Web API, then output Excel file is shown in the image below:

_\[{"color": "red","value": "#f00"},{"color": "green","value": "#0f0"},{"color": "blue","value": "#00f"},{"color": "cyan","value": "#0ff"},{"color": "magenta","value": "#f0f"},{"color": "yellow","value":"#ff0"},{"color": "black","value": "#000"}\]_



{{< figure align=center src="images/OutputExcel.png">}}


### Get Range with External Links

Microsoft Excel supports external links for fetching data from different sources. We have provided the option to retrieve these links from the Excel file using Name.GetRefferedAreas method. This method returns ReferredArea which has many useful properties as follows:

*   EndColumn: The end column of the area
*   EndRow: The end row of the area
*   ExternalFileName: Get the external file name if this is an external reference
*   IsArea: Indicates whether this is an area
*   IsExternalLink: Indicates whether this is an external link
*   SheetName: Indicates which sheet this reference is in
*   StartColumn: The start column of the area
*   StartRow: The start row of the area

You may find details on how to [get range with external links][7] for your reference. In the following example, an external file having named range "Names" is linked with the Excel file. We can access this named range in the linked file and display its properties mentioned above.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Worksheets-GetRangeWithExternalLinks-1.cs" >}}

### Keep Separators for Blank Rows During Spreadsheet to CSV Conversion

Many times you convert the Excel sheets to CSV for using it in some other environment or applications. You may need to decide yourself about the separators for blank rows in the spreadsheet while exporting it to CSV. For example, there is a blank row in the source spreadsheet and you want either a blank row in the CSV or have a row with predefined separators. We have provided this feature now and you can get details about this feature [here][8].

For better understanding, have a look at the following image which shows the result of this feature.



{{< figure align=center src="images/KeepSeparator.png" alt="Import Data from JSON to Excel">}}


Following is a sample code which demonstrates this new feature.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Handling-KeepSeparatorsForBlankRow-1.cs" >}}

To use these useful features and avail other enhancements, I recommend you to try the release [Aspose.Cells for .NET v19.3][9]. And, if you have more time, browse [Developers’ Guide][10] for your complete reference on what you can deliver using the rendering extension API. You are always welcome to share your review, concerns or feedback on [forums][11].




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.3+Release+Notes
[3]: https://apireference.aspose.com/net/cells/aspose.cells/autofitmergedcellstype
[4]: https://docs.aspose.com/display/cellsnet/Autofit+Rows+and+Columns#AutoFitRowsandColumns-AutoFitRowsforMergedCells
[5]: https://docs.aspose.com/display/cellsnet/Tables+and+Ranges#TablesandRanges-ConvertTabletoRangewithOptions
[6]: https://docs.aspose.com/display/cellsnet/Import+Data+into+Worksheet#ImportDataintoWorksheet-ImportingDatafromJSON
[7]: https://docs.aspose.com/display/cellsnet/Get+Range+with+External+Links
[8]: https://docs.aspose.com/display/cellsnet/Keep+Separators+for+Blank+Rows+while+exporting+spreadsheets+to+CSV+format
[9]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.3/
[10]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[11]: https://forum.aspose.com/c/cells




