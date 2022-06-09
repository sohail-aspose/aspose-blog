---
title: 'Add or Remove AutoFilter in Excel Files using C++'
seoTitle: "Add or Remove AutoFilter in Excel Files using C++"
description: "Add and Remove AutoFilter in Excel Files using C++. Add AutoFilters, Date AutoFilters, Dynamic Date AutoFilers, and Custom AutoFilters in Excel Files."
date: Wed, 19 May 2021 13:21:20 +0000
draft: false
url: /2021/05/19/add-or-remove-autofilter-in-excel-files-using-cpp/
author: Muhammad Ahmad
summary: 'Filtering information in Excel spreadsheets is an important feature. It enables you to hide irrelevant data and show only the data meeting specific criteria. There might be scenarios where filtering data can prove to be helpful. For example, an organization may want to filter out low-performing products from the sales report to analyze and improve their sales strategies. In this article, you will learn **how to add or remove AutoFilter in Excel files using C++**.'
tags: ['Add AutoFilter in Excel C++', 'Add Custom AutoFilter in Excel C++', 'Remove AutoFilter from Excel C++']
categories: ['Aspose.Cells Product Family']
---

Filtering information in Excel spreadsheets is an important feature. It enables you to hide irrelevant data and show only the data meeting specific criteria. There might be scenarios where filtering data can prove to be helpful. For example, an organization may want to filter out low-performing products from the sales report to analyze and improve their sales strategies. In this article, you will learn **how to add or remove AutoFilter in Excel files using C++**.

*   [C++ API for Adding and Removing AutoFilter in Excel Files][1]
*   [Apply AutoFilter in Excel Files using C++][2]
*   [Add Date AutoFilter in Excel Files using C++][3]
*   [Add Dynamic Date AutoFilter in an Excel File using C++][4]
*   [Apply Custom AutoFilter in Excel Files using C++][5]
*   [Remove AutoFilter from Excel Files][6]

## C++ API to Adding and Removing AutoFilter in Excel Files {#CPP-API-to-Adding-and-Removing-AutoFilter-in-Excel-Files}

We will use the [Aspose.Cells for C++][7] API for adding and removing AutoFilter in Excel files. It is a native C++ library that allows you to create, read and modify Excel files without requiring Microsoft Excel to be installed. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Apply AutoFilter in Excel Files using C++ {#Apply-AutoFilter-in-Excel-Files-using-CPP}

You can apply AutoFilter on a range of cells. AutoFilters allow you to sort and filter values in the given range of cells. The following are the steps to add AutoFilter in Excel files.

*   Firstly, load the Excel file using the [IWorkbook][10] class.
*   Retrieve the worksheet where you want to apply the AutoFilter using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][11] method.
*   Apply the AutoFilter using the [IWorksheet->GetIAutoFilter()->SetRange(intrusive\_ptr<Aspose::Cells::Systems::String> value)][12] method.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][13] method.

The following sample code shows how to apply AutoFilter to a range of cells in an Excel file using C++.

{{< gist aspose-com-gists d1a6633db176cde4400b1ef1f84d3f90 "Apply-AutoFilter.cpp" >}}



{{< figure align=center src="images/ApplyAutoFilterExcelCpp.png" alt="The image of the output file generated by the sample code" caption="The image of the output file generated by the sample code">}}


## Add Date AutoFilter in Excel Files using C++ {#Add-Date-AutoFilter-in-Excel-Files-using-CPP}

Excel files may contain data based on dates. You might find yourself in scenarios where you need to filter and analyze data based on different dates. Therefore, a date filter will prove to be helpful in such scenarios. The following are the steps to add date AutoFilter in Excel files.

*   Firstly, load the Excel file using the [IWorkbook][14] class.
*   Retrieve the worksheet where you want to apply the AutoFilter using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][15] method.
*   Apply Date AutoFilter using the [IWorksheet->GetIAutoFilter()->AddDateFilter(Aspose::Cells::Systems::Int32 fieldIndex, Aspose::Cells::DateTimeGroupingType dateTimeGroupingType, Aspose::Cells::Systems::Int32 year, Aspose::Cells::Systems::Int32 month, Aspose::Cells::Systems::Int32 day, Aspose::Cells::Systems::Int32 hour, Aspose::Cells::Systems::Int32 minute, Aspose::Cells::Systems::Int32 second)][16] method.
*   To update the worksheet, use the [IWorksheet->GetIAutoFilter()->Refresh()][17] method.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][18] method.

The following sample code demonstrates how to add date AutoFilter in Excel files using C++.

{{< gist aspose-com-gists d1a6633db176cde4400b1ef1f84d3f90 "Apply-Date-AutoFilter.cpp" >}}

## Add Dynamic Date AutoFilter in an Excel File using C++ {#Add-Dynamic-Date-AutoFilter-in-an-Excel-File-using-CPP}

There might be cases where you need a more generic date filter, such as the month irrespective of the year or the month before the current month. For scenarios like this, you can use the dynamic AutoFilter to filter the data. The following are the steps to filter data using a dynamic date AutoFilter.

*   Firstly, load the Excel file using the [IWorkbook][19] class.
*   Retrieve the worksheet where you want to apply the AutoFilter using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][20] method.
*   Apply DynamicFilter using the [IWorksheet->GetIAutoFilter()->DynamicFilter (Aspose::Cells::Systems::Int32 fieldIndex, Aspose::Cells::DynamicFilterType dynamicFilterType)][21] method.
*   To update the worksheet, use the [IWorksheet->GetIAutoFilter()->Refresh()][22] method.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][23] method.

The following sample code demonstrates how to add a dynamic date AutoFilter in an Excel file using C++.

{{< gist aspose-com-gists d1a6633db176cde4400b1ef1f84d3f90 "Apply-Dynamic-Date-AutoFilter.cpp" >}}

## Apply Custom AutoFilter in Excel Files using C++ {#Apply-Custom-AutoFilter-in-Excel-Files-using-CPP}

In case you want to apply a custom AutoFilter, Aspose.Cells for C++ API has you covered. Using the API, you can apply a custom AutoFilter in Excel files based on your specific requirements. The following are the steps to add custom AutoFilter in Excel files.

*   Firstly, load the Excel file using the [IWorkbook][24] class.
*   Retrieve the worksheet where you want to apply the AutoFilter using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][25] method.
*   Apply the Custom AutoFilter using the [IWorksheet->GetIAutoFilter()->Custom(Aspose::Cells::Systems::Int32 fieldIndex, Aspose::Cells::FilterOperatorType operatorType1, intrusive\_ptr<Aspose::Cells::Systems::Object> criteria1)][26] method.
*   Call the [IWorksheet->GetIAutoFilter()->Refresh()][27] method to update the worksheet.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][28] method.

The following sample code shows how to add custom AutoFilter in Excel files using C++.

{{< gist aspose-com-gists d1a6633db176cde4400b1ef1f84d3f90 "Apply-Custom-AutoFilter.cpp" >}}

## Remove AutoFilter from Excel Files {#Remove-AutoFilter-from-Excel-Files}

In the previous sections, you learned how to add different AutoFilters in Excel files. In addition to adding AutoFilters, you can also remove them using the Aspose.Cells for C++ API. The following are the steps to remove AutoFilters from Excel files.

*   Firstly, load the Excel file using the [IWorkbook][29] class.
*   Retrieve the worksheet from where you want to remove the AutoFilter using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][30] method.
*   Remove AutoFilter using the [IWorksheet->RemoveAutoFilter()][31] method.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][32] method.

The following sample code shows how to remove AutoFilter from an Excel file using C++.

{{< gist aspose-com-gists d1a6633db176cde4400b1ef1f84d3f90 "Remove-AutoFilter.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][33].

## Conclusion

In this article, you have learned how to add and remove AutoFilters from Excel files using C++. Specifically, you have learned how to add Default, Date, Dynamic Date and Custom AutoFilters. You have also seen how to remove AutoFilter using Aspose.Cells for C++ API. The API provides many additional features for working with Excel files. You can explore the API in detail by visiting the [official documentation][34]. In case of any questions, please feel free to reach us on our [free support forum][35].

## See Also

*   [Inserting and Deleting Rows and Columns in Excel using C++][36]
*   [Copy or Move Excel Worksheets using C++][37]




[1]: #CPP-API-to-Adding-and-Removing-AutoFilter-in-Excel-Files
[2]: #Apply-AutoFilter-in-Excel-Files-using-CPP
[3]: #Add-Date-AutoFilter-in-Excel-Files-using-CPP
[4]: #Add-Dynamic-Date-AutoFilter-in-an-Excel-File-using-CPP
[5]: #Apply-Custom-AutoFilter-in-Excel-Files-using-CPP
[6]: #Remove-AutoFilter-from-Excel-Files
[7]: https://products.aspose.com/cells/cpp
[8]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[9]: https://downloads.aspose.com/cells/cpp
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a8d7ced178aa0e8638deca4d9b2513f5d
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a1f3fc11eef91c72b43764e03de767e4f
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a79e346d2f49050e75670400a2828ec42
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a6c634d50e7ab7ba1be0ce94bdd8ee8fa
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a79e346d2f49050e75670400a2828ec42
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#ad634cc0e05f99ce05236494c92b77675
[27]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_auto_filter#a79e346d2f49050e75670400a2828ec42
[28]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[29]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[30]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[31]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a90ee992a1a5fb83a5733b905fd3d667a
[32]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[33]: https://purchase.aspose.com/temporary-license
[34]: https://docs.aspose.com/cells/cpp/
[35]: https://forum.aspose.com/c/cells/9
[36]: https://blog.aspose.com/2021/04/23/inserting-and-deleting-rows-and-columns-in-excel-using-cpp/
[37]: https://blog.aspose.com/2021/04/06/copy-or-move-excel-worksheets-using-cpp/




