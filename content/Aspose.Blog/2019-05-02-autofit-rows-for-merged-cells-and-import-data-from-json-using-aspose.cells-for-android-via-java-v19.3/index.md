---
title: 'Autofit Rows for Merged Cells and Import Data from JSON to Excel in Android using Java'
date: Thu, 02 May 2019 09:37:59 +0000
draft: false
url: /2019/05/02/autofit-rows-for-merged-cells-and-import-data-from-json-using-aspose.cells-for-android-via-java-v19.3/
author: Amjad Sahi
summary: ''
tags: ['Autofit Rows for Merged Cells in Excel in Android', 'Convert JSON to Excel in Android', 'JSON to Excel in Android']
categories: ['Aspose.Cells Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100-e1539021448359.png "Aspose.Cells for Android logo") Guys, I'm going to walk you through all the exciting features, improvements and other fixes of [Aspose.Cells for Android via Java v19.3][1]. This release includes new features, enhancements and other bug fixes that further improve the overall stability and usability of the Android API. For an easy access and utilization, Aspose.Cells for Android via Java APIs can be directly installed from Maven repository, see the [document][2] for your reference. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. Let us start reviewing what is there in this release.

### Insert rows with formatting

Microsoft Excel supports a feature to insert a row using one of the three different options. The objective of these options is to adopt settings from other rows. These three options include the following:

*   **Format Same as Above** (copy formatting from the above row)
*   **Format Same as Below** (copy formatting from the row below)
*   **Clear Formatting** (add new row but without any formatting)

You can also see these three options in the following screenshot:



{{< figure align=center src="images/InsertTypes-2.png" alt="Insert a row with one of the three formatting options">}}


The good news is, using Aspose.Cells for Android via Java API, you can use this feature in your code as well. You can programmatically create new rows with specified formatting option. Here is a code sample for you to do just that along the [documentation to insert row with formatting][4]:  
  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-RowsAndColumns-InsertingARowWithFormatting-1.java" >}}

### Replace special chars while opening a CSV file

There was a demand, from you guys, that just like Excel, Aspose.Cells supports [replacing special characters while opening a CSV file][5]. So, we're very excited to break the news that this feature is now supported in the API. Just have a look at the below example to see how easy it is to achieve this with Aspose.Cells for Android via Java.

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-OpeningCSVFilesAndReplacingInvalidCharacters-1.java" >}}

### Detect type of encrypted OOXML files

As you must already have some idea that Office Open XML, which is also known as OOXML or Microsoft Open XML (MOX), is a very common format used for files. It is an XML-based format developed by Microsoft for representing office documents like spreadsheets, charts, presentations, and word processing documents. Aspose.Cells already allowed to open and detect type of this format. But now, our team has gone a step forward, and supported to detect type of encrypted OOXML files. Check out the sample code below:

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-TechnicalArticles-DetectFileFormatOfEncryptedFiles-1.java" >}}  

### Import data from JSON

As you know that JavaScript Object Notation is a common data interchange format which is quite lightweight and can be read by human and machines easily. Now, for example, you get data from some Web API in JSON format and need it to be imported into some Excel file, then Aspose.Cells is there to provide this facility.

JSONUtility class is introduced by Aspose.Cells for this purpose having ImportData method that not only imports data but also performs different conversions and formatting using the JsonLayoutOptions object during the import process. You may try this exciting feature by following article [Importing Data from JSON][6]. Here is a sample code to use this feature:

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Data-ImportingFromJson-1.java" >}}  

You can see that result is cool as fully formatted Excel file is created without using any extra code to parse the JSON string from any source like Web API. Isn't it? For example, if you get the following string from Web API, then output Excel file is shown in the image below:

_\[{"color": "red","value": "#f00"},{"color": "green","value": "#0f0"},{"color": "blue","value": "#00f"},{"color": "cyan","value": "#0ff"},{"color": "magenta","value": "#f0f"},{"color": "yellow","value":"#ff0"},{"color": "black","value": "#000"}\]_



{{< figure align=center src="images/OutputExcel.png" alt="">}}


### Convert table to range with Options

Conversion of the table to a range was available earlier. However what if you want to control the formatting of destination range like formatting only the partial output. The good news is that this feature is available now and you don't need to write extra code to format the output range. We have introduced a new class TableToRangeOptions where LastRow property is available to set the last row to which formatting is copied from the source table. Here is the view of a sample table and converted range which is formatted up to row 5.



{{< figure align=center src="images/RangeTest-1024x375.png" alt="">}}


Here is a sample code which is used to create the above range.

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Tables-ConvertTableToRangeWithOptions-1.java" >}}  

For detailed information on conversions follow [this][7] link.

### Get Range with External Links

Microsoft Excel supports external links for fetching data from different sources. We have provided the option to retrieve these links from the Excel file using [Name.GetRefferedAreas][8] method. This method returns [ReferredArea][9] which has many useful properties as follows:

*   [EndColumn][10]: The end column of the area
*   [EndRow][11]: The end row of the area
*   [ExternalFileName][12]: Get the external file name if this is an external reference
*   [IsArea][13]: Indicates whether this is an area
*   [IsExternalLink][14]: Indicates whether this is an external link
*   [SheetName][15]: Indicates which sheet this reference is in
*   [StartColumn][16]: The start column of the area
*   [StartRow][17]: The start row of the area

In the following example, an external file having named range "Names" is linked with the Excel file. We can access this named range in the linked file and display its properties mentioned above.

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-GetRangeWithExternalLinks-1.java" >}}  

### Keep separators for blank rows during spreadsheet to CSV

Many times you convert the Excel sheets to CSV for using it in some other environment or applications. You may need to decide yourself about the separators for blank rows in the spreadsheet while exporting it to CSV. For example, there is a blank row in the source spreadsheet and you want either a blank row in the CSV or have a row with predefined separators. We have provided this feature now and you can get details about this feature [here][18].

For better understanding, have a look at the following image which shows the result of this feature.



{{< figure align=center src="images/KeepSeparator.png" alt="">}}


Following is a sample code which demonstrates this new feature.

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-KeepSeparatorsForBlankRow-1.java" >}}  

### Autofit Rows for Merged Cells

Autofitting rows is a very common operation which you perform while working with the Excel files. This feature was already there in Aspose.Cells API however many people asked for more control over this operation. To fulfill this requirement we have provided [AutoFitMergedCellsType][19] enumerator which contains the following options:

*   [NONE][20]: Ignore merged cells.
*   [FIRST\_LINE][21]: Only expands the height of the first row.
*   [LAST\_LINE][22]: Only expands the height of the last row.
*   [EACH\_LINE][23]: Expands the height of each row.

Here is a snapshot of this feature where the effect of one of the options EACH\_LINE is shown.



{{< figure align=center src="images/Screenshot-2019-04-18-at-2.48.54-PM.png" alt="">}}


You can test this feature using following sample code.

  
{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-RowsAndColumns-AutofitRowsforMergedCells-1.java" >}}  

For more details on this topic please visit [here][24].

## Useful Links

The resources, you might need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][25].
*   [Aspose.Cells for Android via Java Download Section][26].
*   [Aspose.Cells for Android via Java Documentation][27] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][28] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][29] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][30] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][31] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/19.3/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+Installation#Aspose.CellsforAndroidviaJavaInstallation-InstallAspose.CellsforAndroidviaJavafromMavenRepository
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+19.3+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Inserting+and+Deleting+Rows+and+Columns#InsertingandDeletingRowsandColumns-InsertaRowwithFormatting
[5]: https://docs.aspose.com/display/cellsjava/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningCSVfilesandreplacinginvalidcharacters
[6]: https://docs.aspose.com/display/cellsjava/Import+and+Export+Data#ImportandExportData-ImportingDatafromJSON
[7]: https://docs.aspose.com/display/cellsjava/Convert+an+Excel+Table+to+a+Range+of+Data#ConvertanExcelTabletoaRangeofData-ConvertTabletoRangewithOptions
[8]: https://apireference.aspose.com/java/cells/com.aspose.cells/name#getReferredAreas(boolean)
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/ReferredArea
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#EndColumn
[11]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#EndRow
[12]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#ExternalFileName
[13]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#IsArea
[14]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#IsExternalLink
[15]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#SheetName
[16]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#StartColumn
[17]: https://apireference.aspose.com/java/cells/com.aspose.cells/referredarea#StartRow
[18]: https://docs.aspose.com/display/cellsjava/Keep+Separators+for+Blank+Rows+while+exporting+spreadsheets+to+CSV+format
[19]: https://apireference.aspose.com/java/cells/com.aspose.cells/AutoFitMergedCellsType
[20]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#NONE
[21]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#FIRST_LINE
[22]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#LAST_LINE
[23]: https://apireference.aspose.com/java/cells/com.aspose.cells/autofitmergedcellstype#EACH_LINE
[24]: https://docs.aspose.com/display/cellsjava/Autofit+Rows+and+Columns#AutofitRowsandColumns-AutoFitRowsforMergedCells
[25]: https://www.aspose.com/products/cells/android-java
[26]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/
[27]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[28]: https://apireference.aspose.com/java/cells
[29]: https://forum.aspose.com/c/cells
[30]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[31]: https://github.com/asposecells/Aspose_Cells_Java




