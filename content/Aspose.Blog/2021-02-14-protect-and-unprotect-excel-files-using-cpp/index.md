---
title: 'Protect and Unprotect Excel Files using C++'
seoTitle: "Protect and Unprotect Excel Files using C++ | Password Protect Excel files"
description: "Protect and unprotect Excel files using C++. Protect Excel workbooks using the desired protection level and a custom password within your C++ applications."
date: Sun, 14 Feb 2021 06:38:40 +0000
draft: false
url: /2021/02/14/protect-and-unprotect-excel-files-using-cpp/
author: Muhammad Ahmad
summary: "Microsoft Excel is a popular software for managing data in organizations. It is mainly due to its advanced data manipulation and representation features. In this technological age, documents are shared virtually instead of printed copies. These files may contain complex and sensitive data. So to maintain such files' integrity, you might need to guard them against modification. Excel's protection features come in handy for this purpose. In this article, you will learn **how to protect and unprotect Excel files programmatically using C++**."
tags: ['C++ Protect Excel Workbook', 'Protect Excel files using C++', 'Unprotect Excel File using C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Protect-Excel-Files-C.jpg" alt="Protect and Unprotect Excel Files">}}


Microsoft Excel is a popular software for managing data in organizations. It is mainly due to its advanced data manipulation and representation features. In this technological age, documents are shared virtually instead of printed copies. These files may contain complex and sensitive data. So to maintain such files' integrity, you might need to guard them against modification. Excel's protection features come in handy for this purpose. In this article, you will learn **how to protect and unprotect Excel files programmatically using C++**.

*   [C++ API to Protect and Unprotect Excel Files][1]
*   [Protect Excel Files using C++][2]
*   [Unprotect Excel Workbook using C++][3]
*   [Protect Excel Worksheet using C++][4]
*   [Unprotect Excel Worksheet using C++][5]
*   [Get a Free License][6]

## C++ API to Protect and Unprotect Excel Files - Free Download {#CPP-API-to-Protect-and-Unprotect-Excel-Files-Free-Download}

[Aspose.Cells for C++][7] is a native C++ library that allows you to manipulate Excel files without requiring Microsoft Excel to be installed. Therefore, it is used for automating many Excel workflows. The API provides a bunch of useful features, including protecting and unprotecting Excel files. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Protect Excel Files using C++ {#Protect-Excel-Files-using-CPP}

Aspose.Cells for C++ provides the following protection types for protecting Excel files.

*   **All**: Protect the whole data so that the user cannot modify anything.
*   **Contents**: Protect the content of the worksheet.
*   **Objects**: Protect the objects in the worksheet so that the user cannot modify drawing objects.
*   **Scenarios**: Protect the scenarios in the worksheet.
*   **Structure**: Protect the structure of the workbook.
*   **Windows**: Protect the saved windows from modification.
*   **None**: No protection applied.

The following are the steps for protecting Excel files using C++.

*   Load the Excel file using the [IWorkbook][10] class.
*   Protect the file with [IWorkbook->Protect(Aspose::Cells::ProtectionType protectionType, intrusive\_ptr<Aspose::Cells::Systems::String>password)][11] method.
*   Save the protected Excel file with the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][12] method.

The following code sample shows how to protect Excel files using C++.

{{< gist aspose-com-gists 5219f8e32c7fa3bfdfcc6eb64fd00f42 "Protect-Excel-Files.cpp" >}}

## Unprotect Excel Workbook using C++ {#Unprotect-Excel-Workbook-using-CPP}

The following are the steps to unprotect an Excel file.

*   Load the Excel file using the [IWorkbook][13] class.
*   Unprotect the file with the [IWorkbook->Unprotect(intrusive\_ptr<Aspose::Cells::Systems::String> password)][14] method.
*   Set the password to _NULL_ using the [IWorkbook->GetISettings()->SetPassword(intrusive\_ptr<Aspose::Cells::Systems::String> value)][15] method.
*   Save the unprotected Excel file with the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][16] method.

The following code sample shows how to unprotect Excel files.

{{< gist aspose-com-gists 5219f8e32c7fa3bfdfcc6eb64fd00f42 "Unprotect-Excel-Files.cpp" >}}

## Protect Excel Worksheet using C++ {#Protect-Excel-Worksheet-using-CPP}

In addition to protecting Excel files, you can also protect individual worksheets. Please use the following steps to safeguard Excel worksheets.

*   Firstly, load the Excel file using the [IWorkbook][17] class.
*   Get the worksheet that you want to protect from the worksheet collection using the [IWorkbook->GetIWorksheets()->GetObjectByIndex( Aspose::Cells::Systems::Int32 index)][18] method.
*   Get the worksheet's protection using the [IWorksheet->GetIProtection()][19] method.
*   Set the protection options such as [SetAllowEditingContent (bool value)][20].
*   Set the password using the [IProtection->SetPassword (intrusive\_ptr<Aspose::Cells::Systems::String> value)][21] method.
*   Finally, save the Excel file with the protected worksheet using [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][22] method.

The following code sample shows how to protect Excel worksheet.

{{< gist aspose-com-gists 5219f8e32c7fa3bfdfcc6eb64fd00f42 "Protect-Worksheet.cpp" >}}

## Unprotect Excel Worksheet using C++ {#Unprotect-Excel-Worksheet-using-CPP}

The following are the steps for unprotecting Excel worksheets.

*   Load the Excel file using the [IWorkbook][23] class.
*   Access the protected worksheet using [IWorkbook->GetIWorksheets()->GetObjectByIndex( Aspose::Cells::Systems::Int32 index)][24] method.
*   Unprotect the worksheet using the [IWorksheet->Unprotect(intrusive\_ptr<Aspose::Cells::Systems::String> password)][25] method.
*   Lastly, save the Excel file with the unprotected worksheet using [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][26] method.

The following code sample shows how to unprotect Excel worksheet using C++.

{{< gist aspose-com-gists 5219f8e32c7fa3bfdfcc6eb64fd00f42 "Unprotect-Worksheet.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][27].

## Conclusion

In this article, you have learned how to protect and unprotect Excel files using C++. In addition to that, you have also learned how to guard worksheets against modifications. Aspose.Cells for C++ is a vast Excel manipulation API for automating tasks such as replacing text in cells or processing complex data represented in graphs and charts. You can explore the API in detail by using the [official documentation][28].

## See Also

*   [Convert Excel to HTML using C++][29]




[1]: #CPP-API-to-Protect-and-Unprotect-Excel-Files-Free-Download
[2]: #Protect-Excel-Files-using-CPP
[3]: #Unprotect-Excel-Workbook-using-CPP
[4]: #Protect-Excel-Worksheet-using-CPP
[5]: #Unprotect-Excel-Worksheet-using-CPP
[6]: #Get-a-Free-License
[7]: https://products.aspose.com/cells/cpp
[8]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[9]: https://downloads.aspose.com/cells/cpp
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a3be7a6714351426136fc3460c9768ffe
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#af1cce2d6c7854dfcf44ee34735e9a0a2
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook_settings#a013be738b5ab6aa827d44021c226bbc7
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a75edac7084b51d3902dee1394b27aa35
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_protection#ac2fc092ba93b07279b5c8973979f8ca4
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_protection#aad9cbecee4793b354bf1e2f8d597ae03
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a7f703d04537743b79531d01eb168f9af
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/cells/cpp/
[29]: https://blog.aspose.com/2021/02/06/convert-excel-to-html-using-cpp/





