---
title: 'Copy or Move Excel Worksheets using C++'
seoTitle: "Copy Excel Worksheets using C++ | Move Excel Worksheets using C++"
description: "Copy or Move worksheets in Excel files using C++. Copy an Excel worksheet within the same file or to a different file. Change the position of the worksheet."
date: Tue, 06 Apr 2021 06:35:31 +0000
draft: false
url: /2021/04/06/copy-or-move-excel-worksheets-using-cpp/
author: Muhammad Ahmad
summary: 'Excel files are used for managing complex data such as department budgets or yearly sales reports. There might be situations where you have a ready-made template that you want to use for creating a report. For this, you can create a copy of the template worksheet. You might also need to organize the worksheets to demonstrate the flow of data. For such cases, you can rearrange the worksheets according to your requirements. In light of this, you will learn **how to copy and move worksheets programmatically using C++**.'
tags: ['Copy Worksheet C++', 'Copy Worksheet to Another Workbook C++', 'Move Worksheet C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Copy-Worksheets.jpg" alt="Copy or Move Excel Worksheets">}}


Excel files are used for managing complex data such as departmental budgets or yearly sales reports. There might be situations where you have a ready-made template that you want to use for creating a report. For this, you can create a copy of the template worksheet. You might also need to organize the worksheets to demonstrate the flow of data. For such cases, you can rearrange the worksheets according to your requirements. In light of this, you will learn **how to copy and move worksheets programmatically using C++**.

*   [C++ API to Copy or Move Excel Worksheets][1]
*   [Copy Worksheets within an Excel Workbook using C++][2]
*   [Copy Worksheets from One Workbook to Another][3]
*   [Move the Worksheet to a Different Position using C++][4]
*   [Get a Free License][5]

## C++ API to Copy or Move Excel Worksheets {#CPP-API-to-Copy-or-Move-Excel-Worksheets}

[Aspose.Cells for C++][6] is a native C++ library that allows you to create, read and update Excel files without requiring Microsoft Excel to be installed. The API also supports copying and moving Excel worksheets. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Copy Worksheets within an Excel Workbook using C++ {#Copy-Worksheets-within-an-Excel-Workbook-using-CPP}

The following are the steps to copy worksheets within an Excel workbook.

*   Load the Excel file using the [IWorkbook][9] class.
*   Retrieve the worksheet collection using the [IWorkbook->GetIWorksheets()][10] method.
*   Add the copy of the required worksheet using [IWorksheetCollection->AddCopy (intrusive\_ptr<Aspose::Cells::Systems::String> sheetName)][11] method.
*   Finally, save the Excel file using [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][12] method.

The following is the sample code to copy a worksheet within an Excel workbook using C++.

{{< gist aspose-com-gists c1140967e949c49f1e197bd764a2460b "Copy-Worksheet-Within-Workbook.cpp" >}}

## Copy Worksheets from One Workbook to Another {#Copy-Worksheets-from-One-Workbook-to-Another}

Aspose.Cells for C++ also allows you to copy worksheets between two Excel files. The following are the steps to copy a worksheet from one Excel file to another.

*   Firstly, load the source and destination Excel files using the [IWorkbook][13] class.
*   Retrieve the worksheet collection of the source workbook using the [IWorkbook->GetIWorksheets()][14] method.
*   Retrieve the worksheet you want to copy using [IWorksheetCollection->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][15] method.
*   Copy the worksheet to the destination workbook using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)->Copy (intrusive\_ptr<Aspose::Cells::IWorksheet> sourceSheet)][16] method.
*   Finally, save the destination Excel file using [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][17] method.

The following is the sample code to copy a worksheet from one Excel workbook to another using C++.

{{< gist aspose-com-gists c1140967e949c49f1e197bd764a2460b "Copy-Worksheet-Between-Workbooks.cpp" >}}

## Move the Worksheet to a Different Position using C++ {#Move-the-Worksheet-to-a-Different-Position-using-CPP}

The following are the steps to change the position of the worksheet within an Excel Workbook.

*   Load the Excel file using the [IWorkbook][18] class.
*   Retrieve the worksheet collection using the [IWorkbook->GetIWorksheets()][19] method.
*   Retrieve the worksheet you want to move using [IWorksheetCollection->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][20] method.
*   Move the worksheet to the desired location using [IWorksheet->MoveTo (Aspose::Cells::Systems::Int32 index)][21] method.
*   Finally, save the Excel file using [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][22] method.

The following is the sample code to move the worksheet to a different position within the same workbook using C++.

{{< gist aspose-com-gists c1140967e949c49f1e197bd764a2460b "Move-Worksheet-Within-Workbook.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][23].

## Conclusion

In this article, you have learned how to copy worksheets within the same Excel workbook or between different workbooks. Furthermore, you have seen how to change the position of the worksheet within an Excel file. Aspose.Cells for C++ provides many more features for working with Excel files that you can explore by visiting the [official documentation][24]. In case of any questions, please feel free to reach us on our [free support forum][25].

## See Also

*   [Convert Excel Files to Images using C++][26]
*   [Create MS Excel Spreadsheets in C++ without MS Office][27]




[1]: #CPP-API-to-Copy-or-Move-Excel-Worksheets
[2]: #Copy-Worksheets-within-an-Excel-Workbook-using-CPP
[3]: #Copy-Worksheets-from-One-Workbook-to-Another
[4]: #Move-the-Worksheet-to-a-Different-Position-using-CPP
[5]: #Get-a-Free-License
[6]: https://products.aspose.com/cells/cpp
[7]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[8]: https://downloads.aspose.com/cells/cpp
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a72a58bea6003036e79282f54e0bfcffc
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#aa1e73c54ea19bb7aa0f9f197c2baa5ba
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a72a58bea6003036e79282f54e0bfcffc
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#ae95f6a0ec074f5583d6ff5b487facbab
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a72a58bea6003036e79282f54e0bfcffc
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a240bf1d3d52ea8c8bfd54ffa320921b7
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/cells/cpp/
[25]: https://forum.aspose.com/c/cells/9
[26]: https://blog.aspose.com/2021/01/28/convert-excel-files-to-images-using-cpp/
[27]: https://blog.aspose.com/2020/05/15/create-ms-excel-spreadsheets-xls-xlsx-in-cpp-without-ms-office/





