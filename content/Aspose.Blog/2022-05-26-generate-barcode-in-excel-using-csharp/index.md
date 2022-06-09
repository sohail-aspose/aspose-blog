---
title: 'Generate Barcode in Excel using C#'
seoTitle: "Generate Barcode in Excel using C# | Read Barcode from Excel using C#"
description: "Programmatically Generate Barcode in Excel using C# with Aspose.BarCode for .NET API. Recognize and read barcodes from Excel spreadsheets using C#."
date: Thu, 26 May 2022 08:42:04 +0000
draft: false
url: /2022/05/26/generate-barcode-in-excel-using-csharp/
author: Muzammil Khan
summary: 'You can easily add a machine-readable barcode image to an XLSX or XLS file programmatically in .NET applications. In this article, you will learn **how to generate a barcode in Excel using C#**.'
tags: ['Add Barcode in Excel C#', 'Add Barcode to Excel File C#', 'Add QR Code in Excel', 'Add QR code in Excel using C#', 'Barcode in Excel', 'C# API to Generate Barcode in Excel', 'Generate Barcode in Excel', 'Read Barcode from Excel', 'Read Barcode from Excel using C#']
categories: ['Aspose.Cells Product Family', 'Aspose.BarCode Product Family']
---



{{< figure align=center src="images/generate-barcode-in-excel-using-csharp.jpg" alt="Generate Barcode in Excel using C#">}}


Excel is a [spreadsheet][1] application developed and published by Microsoft. It is most commonly used to store, organize, and track data sets with formulas and functions. In certain cases, we may need to generate and add barcodes in Excel files to embed specific information. We can add machine-readable barcode images to [XLSX][2] or [XLS][3] files programmatically in .NET applications. In this article, we will learn **how to generate a barcode in Excel using C#**.

The article shall cover the following topics:

*   [C# API to Generate Barcode in Excel][4]
*   [Create Excel Spreadsheet and Add Barcode][5]
*   [Add Barcode to Existing Excel File][6]
*   [Add QR Code to Excel File][7]
*   [Read Barcode from Excel File][8]

## C# API to Generate Barcode in Excel {#CSharp-API-to-Generate-Barcode-in-Excel}

For adding barcodes to Excel spreadsheets, we will follow a two-step procedure. We will be using the [Aspose.Cells for .NET][9] API to create or load an Excel file. The _[Workbook][10]_ class of the API allows creating a new Excel workbook or loading an existing Excel file for further processing. The _[Save()][11]_ method of this class saves the Workbook on the given file path. The API also provides a _[Worksheet][12]_ class to handle all the sheet-level operations.

We will generate and add the barcode image to the Excel sheet using the [Aspose.BarCode for .NET][13] API. It provides the _[BarcodeGenerator][14]_ class to generate the barcode of the specified _[EncodeType][15]_. The [_Save()_][16] method of this class saves the barcode image to stream in a specific format. It provides _[BarCodeImageFormat][17]_ enumeration to specify the save formats. The API also provides the _[BarCodeReader][18]_ class to read the barcode from images.

Please either [download][19] the DLLs of the APIs or install them using [NuGet][20].

```
PM> Install-Package Aspose.BarCode
PM> Install-Package Aspose.Cells
```

## Create Excel Spreadsheet and Add Barcode in C# {#Create-Excel-Spreadsheet-and-Add-Barcode-in-CSharp}

We can create a new Excel spreadsheet and add a barcode image to the Excel by following the steps given below:

1.  Firstly, create an instance of the **_BarcodeGenerator_** class with the _**EncodeType**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object.
3.  Then, call the **_Save()_** method to save the barcode image to the memory stream.
4.  Next, create an instance of the **_Workbook_** class.
5.  Then, add a new **_Worksheet_** to the **_[WorksheetCollection][21]_** of the **_Workbook_**.
6.  After that, add the image to the **_[PictureCollection][22]_** of the **_Worksheet_** with the stream object and image position as arguments.
7.  Finally, call the **_Save()_** method. It takes the output XLSX file path as an argument.

The following code example demonstrates **how to create a new Excel spreadsheet and add a barcode image using C#**.

{{< gist aspose-barcode-gists c1cd80387158db0d6e75cf5aa74bf734 "Generate-Barcode-in-Excel-CSharp_Add.cs" >}}



{{< figure align=center src="images/Create-Excel-Spreadsheet-and-Add-Barcode-in-CSharp.jpg" alt="Create an Excel Spreadsheet and Add a Barcode using C#." caption="Create an Excel Spreadsheet and Add a Barcode using C#.">}}


## Add Barcode to Existing Excel File in C# {#Add-Barcode-to-Existing-Excel-File-in-CSharp}

We can also add a barcode image to any sheet of an existing Excel workbook by following the steps given below:

1.  Firstly, create an instance of the **_BarcodeGenerator_** class with the _**EncodeType**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object.
3.  Then, call the **_Save()_** method to save the barcode image to the memory stream.
4.  Next, load an existing Excel file using the **_Workbook_** class.
5.  Then, access the **_Worksheet_** by its index.
6.  After that, add the image to the **_PictureCollection_** using the **_Add()_** method with the stream object and image position as arguments.
7.  Finally, call the **_Save()_** method. It takes the output XLSX file path as an argument.

The following code example demonstrates **how to add a barcode image to an existing Excel file using C#**.

{{< gist aspose-barcode-gists c1cd80387158db0d6e75cf5aa74bf734 "Generate-Barcode-in-Excel-CSharp_AddToExisting.cs" >}}

## Add QR Code to Excel File in C# {#Add-QR-Code-to-Excel-File-in-CSharp}

Similarly, we can also add a QR code to the Excel file by following the steps mentioned earlier. However, we just need to set the _**EncodeType**_ as _**QR**_ in the first step. We may also need to adjust the image position in step # 6.

The following code example demonstrates **how to add a QR code to an Excel file using C#**.

{{< gist aspose-barcode-gists c1cd80387158db0d6e75cf5aa74bf734 "Generate-Barcode-in-Excel-CSharp_AddQR.cs" >}}

## Read Barcode from Excel File using C# {#Read-Barcode-from-Excel-File-using-CSharp}

We can recognize any barcode image embedded on any sheet of the Excel file by following the steps given below:

1.  Firstly, load an existing Excel file using the **_Workbook_** class.
2.  Then, access the **_Worksheet_** by its index.
3.  Next, save the images to stream from **_PictureCollection_** in a loop.
4.  Next, create an instance of the **_BarCodeReader_** class with image stream and **_[DecodeType][23]_** as arguments.
5.  After that, call the **_[ReadBarCodes()][24]_** method to get the **_[BarCodeResult][25]_** object.
6.  Finally, show the barcode information.

The following code example demonstrates **how to read a barcode image from an Excel file using C#**.

{{< gist aspose-barcode-gists c1cd80387158db0d6e75cf5aa74bf734 "Generate-Barcode-in-Excel-CSharp_Read.cs" >}}

The above code sample shall produce the following output.

```
Codetext found: Code128
Symbology: 1234567
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][26] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create an Excel workbook programmatically;
*   add a new sheet in the Excel workbook;
*   generate and add a barcode image to the Excel spreadsheet;
*   read a barcode image from an Excel file.

Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][27]. In case of any ambiguity, please feel free to contact us on the [forum][28].

## See Also

*   [Add Barcode to PDF using C#][29]
*   [Generate Barcode with Logo using C#][30]
*   [Generate and Display Barcode Image in ASP.NET MVC][31]




[1]: https://docs.fileformat.com/spreadsheet/
[2]: https://docs.fileformat.com/spreadsheet/xlsx/
[3]: https://docs.fileformat.com/spreadsheet/xls/
[4]: #CSharp-API-to-Generate-Barcode-in-Excel
[5]: #Create-Excel-Spreadsheet-and-Add-Barcode-in-CSharp
[6]: #Add-Barcode-to-Existing-Excel-File-in-CSharp
[7]: #Add-QR-Code-to-Excel-File-in-CSharp
[8]: #Read-Barcode-from-Excel-File-using-CSharp
[9]: https://products.aspose.com/cells/net
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/save
[12]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet/
[13]: https://products.aspose.com/barcode/net/
[14]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/2
[17]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodeimageformat/
[18]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[19]: https://downloads.aspose.com/barcode/net
[20]: https://www.nuget.org/packages/aspose.barcode
[21]: https://apireference.aspose.com/cells/net/aspose.cells/worksheetcollection/
[22]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/picturecollection/
[23]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/constructors/2
[24]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[25]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/barcode/net/
[28]: https://forum.aspose.com/c/barcode/13
[29]: https://blog.aspose.com/2022/05/14/add-barcode-to-pdf-using-csharp/
[30]: https://blog.aspose.com/2022/04/23/generate-barcode-with-logo-using-csharp/
[31]: https://blog.aspose.com/2022/04/04/generate-and-display-barcode-image-in-asp-net-mvc/




