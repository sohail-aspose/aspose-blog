---
title: 'Find and Replace Text in Excel Spreadsheets using C++'
seoTitle: "Find and Replace Text in Excel Spreadsheets using C++"
description: "Find and replace text in Excel files using C++. Use Aspose.Cells for C++ API to find and replace text in XLSX, XLS files within your C++ applications."
date: Thu, 11 Feb 2021 10:42:41 +0000
draft: false
url: /2021/02/11/find-and-replace-text-in-excel-spreadsheets-using-cpp/
author: Muhammad Ahmad
summary: "Microsoft Excel allows you to store data in tabular form. In addition to that, it enables you to perform complex operations on data. Excel's uses range from maintaining monthly budgets to managing organizational data due to its vast set of features. As compared to other features, finding and replacing text is among the more straightforward tasks you can do in Excel. This article demonstrates how to find and replace text in Excel spreadsheets programmatically using C++."
tags: ['C++ Find and Replace text in Excel', 'Find and Replace text in Excel', 'Find and Replace text in XLS files', 'Find and Replace text in XLSX files']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-Excel.png" alt="Find and Replace Text in Excel C++">}}


Microsoft Excel allows you to store data in tabular form. In addition to that, it enables you to perform complex operations on data. Excel's uses range from maintaining monthly budgets to managing organizational data due to its vast set of features. As compared to other features, finding and replacing text is among the more straightforward tasks you can do in Excel. This article demonstrates **how to find and replace text in Excel spreadsheets programmatically using C++**.

*   [C++ API to Find and Replace Text in Excel Files][1]
*   [Finding and Replacing Text in Excel Files using C++][2]
*   [Get a Free License][3]

## C++ API to Find and Replace Text in Excel Files {#CPP-API-to-Find-and-Replace-Text-in-Excel-Files}

[](https://products.aspose.com/cells/cpp)[Aspose.Cells for C++][4] is a robust API for generating, transforming, and managing Excel files. It allows you to automate various aspects of spreadsheet workflows. The API also simplifies finding and replacing text in Excel files. You can either install the API through [NuGet][5] or download it directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Find and Replace Text in Excel Files using C++ {#Find-and-Replace-Text-in-Excel-Files-using-CPP}

The following are the steps for finding and replacing text in Excel files.

*   Load the Excel file using the [IWorkbook][7] class.
*   Create an instance of the [IReplaceOptions][8] class.
*   Set the case sensitivity for searching the text with [IReplaceOptions->SetCaseSensitive(bool _value_)][9] method. By setting this option to _true_, the API will replace only the text with the matching case.
*   Set the option for matching the entire contents of the cell with [IReplaceOptions->SetMatchEntireCellContents(bool _value_)][10] method. By setting this option to _true_, the API will replace text in only the cells containing the exact placeholder text (the text you want to replace).
*   Call the [IWorkbook->Replace( intrusive\_ptr<Aspose::Cells::Systems::String> _placeHolder_, intrusive\_ptr<Aspose::Cells::Systems::String> _newValue_, intrusive\_ptr<Aspose::Cells::IReplaceOptions> _options_)][11] method to replace the text.
*   Save the updated spreadsheet using [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> _fileName_)][12] method.

The following code sample shows how to find and replace text in spreadsheets.

{{< gist aspose-com-gists 20bea3a300043930ddaff689d1629fd5 "Find-and-replace-text-in-Excel.cpp" >}}



{{< figure align=center src="images/FindAndReplaceTextExcel.png" alt="Image comparing files before and after text replacement" caption="Image comparing source and output files">}}


## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][13].

## Conclusion

In this article, you have learned how to find and replace text in Excel files. Furthermore, you have seen how to set additional options like case-sensitivity and matching the entire cell's contents for finding text. Other than this, the API provides a bunch of features for working with Excel files. You can explore Aspose.Cells for C++ API in detail by using the [official documentation][14].

## See Also

*   [Convert Excel Files to PDF using C++][15]




[1]: #CPP-API-to-Find-and-Replace-Text-in-Excel-Files
[2]: #Find-and-Replace-Text-in-Excel-Files-using-CPP
[3]: #Get-a-Free-License
[4]: https://products.aspose.com/cells/cpp
[5]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[6]: https://downloads.aspose.com/cells/cpp
[7]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[8]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_replace_options
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_replace_options#aba527e4439a4a298c354b50ca454eab6
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_replace_options#a3d9a8779a366294ba683411e413d2d77
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#ae4223e4a59b35832da58f17cfcd52673
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/cells/cpp/
[15]: https://blog.aspose.com/2021/01/19/Convert-Excel-to-PDF-using-Cpp/





