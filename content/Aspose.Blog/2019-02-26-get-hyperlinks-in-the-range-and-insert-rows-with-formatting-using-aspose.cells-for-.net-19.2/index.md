---
title: 'Get Hyperlinks in Cell Range and Insert Rows with Formatting using C#'
date: Tue, 26 Feb 2019 17:22:00 +0000
draft: false
url: /2019/02/26/get-hyperlinks-in-the-range-and-insert-rows-with-formatting-using-aspose.cells-for-.net-19.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

Sometimes you got to give values to smaller yet important tasks while generating spreadsheets. In this release, [Aspose.Cells for .NET v19.2][1] offers you a few compact features and other enhancements. You can find a quick way to get hyperlinks in the range is not so difficult. Moreover, no hindrance is imposed regarding styles/formatting while inserting new rows/columns. So, let's not wait another moment to review the [release notes][2] to know all the valuable features and enhancements. I will exhibit a few valuable features and other enhancements with details.

### Get Hyperlinks in the Range

Aspose.Cells for .NET does provide utility features every now and then for the users. In this respect, we have enhanced the Range class that provides a Hyperlinks property which returns all the hyperlinks in the selected range. You may easily traverse the hyperlinks collection to get all the links in the range cells. See the [document][3] with sample code for your reference.

## Insert Rows with Formatting

Microsoft Excel supports a feature to insert a row using one of the three different options. The objective of these options is to adopt settings from other rows. These three options include the following:

*   **Format Same as Above** (copy formatting from the above row)
*   **Format Same as Below** (copy formatting from the row below)
*   **Clear Formatting** (add new row but without any formatting)

You can also see these three options in the following screenshot:



{{< figure align=center src="images/InsertTypes-2.png" alt="Insert a row with one of the three formatting options">}}


The good news is, using Aspose.Cells, you can use this feature in your code as well. You can programmatically create new rows with specified formatting option. Here is a code sample for you to do just that along the [documentation to insert row with formatting][4]:

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-RowsColumns-InsertingAndDeleting-InsertingARowWithFormatting-1.cs" >}}

## Replace Special Chars while Opening a CSV File

There was a demand, from you guys, that just like Excel, Aspose.Cells supports [replacing special characters while opening a CSV file][5]. So, we're very excited to break the news that this feature is now supported in the API. Just have a look at the below example to see how easy it is to achieve this with Aspose.Cells for .NET.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Handling-OpeningCSVFilesAndReplacingInvalidCharacters-1.cs" >}}

## Detect Type of Encrypted OOXML Files

As you must already have some idea that Office Open XML, which is also known as OOXML or Microsoft Open XML (MOX), is a very common format used for files. It is an XML-based format developed by Microsoft for representing office documents like spreadsheets, charts, presentations, and word processing documents. Aspose.Cells already allowed to open and detect type of this format. But now, our team has gone a step forward, and supported to detect type of encrypted OOXML files. Check out the sample code below:

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Utility-DetectFileFormatOfEncryptedFiles-1.cs" >}}

## Other Enhancements

In addition to the features highlighted above, you can now improve your products with the help of these 3 major improvements:

*   A few enhancements are included for setting Box Whisker chart styles (Advanced MS Excel chart types).
*   Based on our user's demand to **a_ccess all the hyperlinks in a range of cells and delete_** anyone if required, we have supported this feature in this release. You can use **Range.Hyperlinks** attribute to get all the hyperlinks from a range, and then delete those using **Hyperlink.Delete()** method.
*   Small integer variable was available to get the number of cells in the Worksheet. In the newer versions of Excel, when number of cells was increased, it was not possible to **_get the large number of cells_**. This shortcoming is corrected by providing appropriate data type which can be evaluated using [sample code in this topic][6].

## A Few Minor Changes in the API

The following is a list of some minor changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible changes made to Aspose.Cells for .NET:

*   Added **ListObject.AlternativeDescription** and **ListObject.AlternativeText** properties toget and set the alternative text and description of the table
*   Added **Line.ThemeColor property** to get and set the theme color of the line
*   Added **Mode3d** and **MsoModel3dFormat** class which encapsulates the object that represents a single 3D model in a spreadsheet
*   Added **ImageType.Gltf enum** which represents the type of 3D model.




[1]: https://www.nuget.org/packages/Aspose.Cells/19.2.0
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.2+Release+Notes
[3]: https://docs.aspose.com/display/cellsnet/Get+Hyperlinks+in+Range
[4]: https://docs.aspose.com/display/cellsnet/Inserting+and+Deleting+Rows+and+Columns#InsertingandDeletingRowsandColumns-InsertaRowwithFormatting
[5]: https://docs.aspose.com/display/cellsnet/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningCSVfilesandreplacinginvalidcharacters
[6]: https://docs.aspose.com/display/cellsnet/Count+number+of+cells+in+the+Worksheet




