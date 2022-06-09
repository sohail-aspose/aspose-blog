---
title: 'Add Comments in Excel Worksheets using C++'
seoTitle: "Add Comments in Excel Worksheets using C++ | Format Comments"
description: "Add comments to a cell in an Excel worksheet using C++. Format cell comments in Excel worksheets programmatically using C++."
date: Mon, 06 Sep 2021 16:24:25 +0000
draft: false
url: /2021/09/06/add-comments-in-excel-worksheets-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft Excel provides the option to add comments in Excel files. There can be several reasons for adding comments, such as explaining a formula or adding contextual information that might be useful to the reader. Comments may also be used to suggest edits in the worksheet. Furthermore, you can set the font size, height, width, etc., of the comments. In this article, you will learn **how to add comments to Excel worksheets programmatically using C++**.'
tags: ['Add Comments in Excel Worksheet C++', 'Cells C++ API', 'Format comment in Excel Worksheet C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Comments-in-Excel.jpg" alt="Add Comments in Excel Worksheets using C++">}}


Microsoft Excel provides the option to add comments in Excel files. There can be several reasons for adding comments, such as explaining a formula or adding contextual information that might be useful to the reader. Comments may also be used to suggest edits in the worksheet. Furthermore, you can set the font size, height, width, etc., of the comments. In this article, you will learn **how to add comments to Excel worksheets programmatically using C++**.

*   [C++ API for Adding Comments in Excel Worksheets][1]
*   [Add Comments in an Excel Worksheet using C++][2]
*   [Apply Formatting to Comments in an Excel Worksheet using C++][3]

## C++ API for Adding Comments in Excel Worksheets {#CPP-API-for-Adding-Comments-in-Excel-Worksheets}

[Aspose.Cells for C++][4] is a native C++ library that allows you to work with Excel files. With the API, you can easily create, read and modify Excel files. Furthermore, you can add comments to your Excel worksheets. To get started, install the API through [NuGet][5] or download it directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Add Comments in an Excel Worksheet using C++ {#Add-Comments-in-an-Excel-Worksheet-using-CPP}

The following are the steps to add a comment to a cell in an Excel worksheet.

*   Load the Excel file using the [IWorkbook][7] class.
*   Retrieve the worksheet where you want to add the comment.
*   Add the comment using the [IWorksheet->GetIComments()->Add(intrusive\_ptr<Aspose::Cells::Systems::String> cellName)][8] method.
*   Retrieve the comment added in the previous step using the [IWorksheet->GetIComments()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][9] method.
*   Set the note of the comment using the [IComment->SetNote(intrusive\_ptr<Aspose::Cells::Systems::String> value)][10] method.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][11] method.

The following sample code shows how to add a comment to a cell in an Excel worksheet using C++.

{{< gist aspose-com-gists 3fba100568c3e5988c396dd0630449d2 "Add_Comment.cpp" >}}



{{< figure align=center src="images/AddCommentExcelCPP.jpg" alt="Image showing the comment added to the cell F5" caption="Image showing the comment added to the cell F5[](https://blog.aspose.com/wp-content/uploads/sites/2/2021/09/AddCommentExcelCPP.jpg)">}}


## Apply Formatting to Comments in an Excel Worksheet using C++ {#Apply-Formatting-to-Comments-in-an-Excel-Worksheet-using-CPP}

The following are the steps to apply formatting to comments in an Excel worksheet using C++.

*   Load the Excel file using the [IWorkbook][12] class.
*   Retrieve the worksheet where you want to add the comment.
*   Add the comment using the [IWorksheet->GetIComments()->Add(intrusive\_ptr<Aspose::Cells::Systems::String> cellName)][13] method.
*   Retrieve the comment added in the previous step using the [IWorksheet->GetIComments()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][14] method.
*   Set the note of the comment using the [IComment->SetNote(intrusive\_ptr<Aspose::Cells::Systems::String> value)][15] method.
*   Set the formatting of the comment according to your needs.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][16] method.

The following sample code shows how to apply formatting to a comment in an Excel worksheet using C++.

{{< gist aspose-com-gists 3fba100568c3e5988c396dd0630449d2 "Apply_Formatting_To_Comment.cpp" >}}



{{< figure align=center src="images/ApplyFormattingToCommentExcelCPP.jpg" alt="Image showing the comment with custom formatting added to the cell F5" caption="Image showing the comment with custom formatting added to the cell F5">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][17].

## Conclusion

In this article, you have learned how to add comments in an Excel worksheet using C++. Furthermore, you have seen how to apply formatting to comments using the simple to use Aspose.Cells for C++ API. The API provides a bunch of additional features for working with Excel files that you can explore in detail by visiting the [official documentation][18]. In case of any questions, please feel free to reach us at our [free support forum][19].

## See Also

*   [Add or Remove AutoFilter in Excel Files using C++][20]
*   [Copy or Move Excel Worksheets using C++][21]




[1]: #CPP-API-for-Adding-Comments-in-Excel-Worksheets
[2]: #Add-Comments-in-an-Excel-Worksheet-using-CPP
[3]: #Apply-Formatting-to-Comments-in-an-Excel-Worksheet-using-CPP
[4]: https://products.aspose.com/cells/cpp
[5]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[6]: https://downloads.aspose.com/cells/cpp
[7]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[8]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment_collection#a3f014415e292fa15c6220e9727dad384
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment_collection#a253830b55bde03d3fa70dba51635be90
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment#a791b9d4e9bf3975709a7f93b5db09580
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment_collection#a3f014415e292fa15c6220e9727dad384
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment_collection#a253830b55bde03d3fa70dba51635be90
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_comment#a791b9d4e9bf3975709a7f93b5db09580
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/cpp/
[19]: https://forum.aspose.com/c/cells/9
[20]: https://blog.aspose.com/2021/05/19/add-or-remove-autofilter-in-excel-files-using-cpp/
[21]: https://blog.aspose.com/2021/04/06/copy-or-move-excel-worksheets-using-cpp/




