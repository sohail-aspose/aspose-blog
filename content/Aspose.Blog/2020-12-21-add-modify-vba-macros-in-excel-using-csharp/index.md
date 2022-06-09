---
title: 'Add or Modify VBA Macros in Excel Files using C#'
seoTitle: ""
description: ""
date: Mon, 21 Dec 2020 19:00:57 +0000
draft: false
url: /2020/12/21/add-modify-vba-macros-in-excel-using-csharp/
author: Usman Aziz
summary: '[VBA][1] (Visual Basic for Applications) is a programming language that is used in MS Excel files in order to automate the spreadsheets related operations. VBA macros are used to write user-defined functions that let you speed up the tasks you have to perform manually. In this article, you will learn how to work with VBA macros in MS Excel files programmatically. By the end of this article, you will be able to **extract, add, and modify VBA macros in Excel workbooks using C#**.'
tags: ['add vba macro in excel using csharp', 'extract vba macro in excel using csharp', 'modify vba macro in excel using csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Work-with-VBA-Macros.jpg" alt="Work with VBA Macro in C#">}}


[VBA][2] (Visual Basic for Applications) is a programming language that is used in MS Excel files in order to automate spreadsheets related operations. VBA macros are used to write user-defined functions that let you speed up the tasks you have to perform manually. In this article, you will learn how to work with VBA macros in MS Excel files programmatically. By the end of this article, you will be able to **extract, add, and modify VBA macros in Excel workbooks using C#**.

*   [Work with VBA Macros using C# API][3]
*   [Extract VBA Macros from an Excel Workbook][4]
*   [Add VBA Macros to an Excel Workbook][5]
*   [Modify VBA Macro in an Excel Workbook][6]
*   [Get a Free License][7]

**TIP**

You may want to check out **Aspose** [FREE macro removal web app][8].

## Work with VBA Macros in Excel Files - C# API {#Manipulate-VBA-Macros-using-CSharp-API}

[Aspose.Cells for .NET][9] is a C# class library that is designed to automate spreadsheet manipulation from within the .NET applications. The API provides a wide range of features that empower you to create, modify, and convert MS Excel workbooks. In addition, the API makes it possible to work with VBA macros seamlessly. Aspose.Cells for .NET is available for [download][10] as a DLL file as well as hosted on [NuGet][11].

```
PM> Install-Package Aspose.Cells
```

## Extract VBA Macros from an Excel File using C# {#Extract-VBA-Macros-form-an-Excel-Workbook}

Let's start by extracting the VBA macros from an existing Excel workbook. The following are the steps to perform this operation.

*   Create an object of the [Workbook][12] class to load the Excel file.
*   Access each VBA module from [Workbook.VbaProject.Modules][13] collection into [VbaModule][14] object.
*   Retrieve code from each module using [VbaModule.Codes][15] property.

The following code sample shows how to extract VBA macro from an Excel workbook using C#.

{{< gist aspose-com-gists 472b011882a191b709e23e7780c2b575 "extract-vba-macro-in-excel.cs" >}}

## Add VBA Macros to an Excel File using C# {#Add-VBA-Macros-to-an-Excel-Workbook}

Aspose.Cells for .NET also allows you to add VBA macros to existing or new Excel files. This can be done by following the below steps.

*   Create a new Excel file or load an existing one using [Workbook][16] class.
*   Add a new worksheet or get the existing one using [Worksheet][17] class.
*   Add a new VBA module using [Workbook.VbaProject.Modules.Add(Worksheet)][18] method and get the module's ID.
*   Access the VBA module from [Workbook.VbaProject.Modules\[idx\]][19] collection into [VbaModule][20] object.
*   Add the name of the module using [VbaModule.Name][21] property.
*   Add code to the module using [VbaModule.Codes][22] property.
*   Save the workbook using [Workbook.Save(String, SaveFormat.Xlsm)][23] method.

The following code sample shows how to add a VBA macro to Excel workbook using C#.

{{< gist aspose-com-gists 472b011882a191b709e23e7780c2b575 "add-vba-macro-in-excel.cs" >}}

## Modify VBA Macro in an Excel File using C# {#Modify-VBA-Macro-in-an-Excel-Workbook}

You can also modify the existing VBA macros in an Excel file using the following steps.

*   Use [Workbook][24] class to load the Excel file.
*   Access the VBA modules from [Workbook.VbaProject.Modules][25] collection into [VbaModule][26] object.
*   Retrieve code from the desired module using [VbaModule.Codes][27] property.
*   Replace the code and save the Excel file using [Workbook.Save(String)][28] method.

The following code sample shows how to modify a VBA macro in an Excel file using C#.

{{< gist aspose-com-gists 472b011882a191b709e23e7780c2b575 "modify-vba-macro-in-excel.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use or evaluate Aspose.Cells for .NET for free using a temporary license valid for 30 days. [Get yours now][29].

## Conclusion

VBA macros in MS Excel files are used to automate various types of tasks related to spreadsheets. In order to handle VBA macros programmatically, this article covered how to extract, add, and modify code in VBA modules using C#. You can explore more about the C# spreadsheet manipulation API using [documentation][30].

## See Also

*   [Protect or Unprotect Excel Files using C#][31]




[1]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[2]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[3]: #Manipulate-VBA-Macros-using-CSharp-API
[4]: #Extract-VBA-Macros-form-an-Excel-Workbook
[5]: #Add-VBA-Macros-to-an-Excel-Workbook
[6]: #Modify-VBA-Macro-in-an-Excel-Workbook
[7]: #Get-a-Free-License
[8]: https://products.aspose.app/slides/remove-macros
[9]: https://products.aspose.com/cells/net
[10]: https://downloads.aspose.com/cells/net
[11]: http://nuget.org/packages/Aspose.Cells
[12]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbaproject/properties/modules
[14]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule
[15]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule/properties/codes
[16]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[17]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[18]: https://apireference.aspose.com/cells/net/aspose.cells.vba.vbamodulecollection/add/methods/1
[19]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbaproject/properties/modules
[20]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule
[21]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule/properties/name
[22]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule/properties/codes
[23]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[24]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[25]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbaproject/properties/modules
[26]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule
[27]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbamodule/properties/codes
[28]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/cells/net/developer-guide/
[31]: https://blog.aspose.com/2020/12/14/protect-or-unprotect-excel-files-using-csharp/





