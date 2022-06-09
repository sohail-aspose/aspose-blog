---
title: 'Protect VBA Macros in Excel using C#'
seoTitle: "C# Protect VBA Macros in Excel | Password Protect Excel VBA Projects"
description: "Use .NET API to protect VBA macros in Excel files using C#. Apply password protection to VBA projects in Excel files in ASP.NET or other .NET applications."
date: Tue, 06 Apr 2021 11:14:00 +0000
draft: false
url: /2021/04/06/protect-vba-macros-in-excel-using-csharp/
author: Usman Aziz
summary: 'VBA macros in Excel spreadsheets are used to automate different operations programmatically. For example, you can program a task that is to be done repeatedly, generate graphs using code, etc. However, the protection of VBA macros from unauthorized users is an important aspect. In order to handle this issue, this article covers **how to protect VBA macros in Excel spreadsheets programmatically using C#**.'
tags: ['password protect Excel VBA project in csharp', 'protect Excel VBA project in csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Work-with-VBA-Macros.jpg" alt="protect Excel VBA C#">}}


VBA macros in Excel spreadsheets are used to automate different operations programmatically. For example, you can program a task that is to be done repeatedly, generate graphs using code, etc. However, the protection of VBA macros from unauthorized users is an important aspect. In order to handle this issue, this article covers **how to protect VBA macros in Excel spreadsheets programmatically using C#**.

*   [API to Protect Excel VBA Macros][1]
*   [Protect Excel VBA Macros][2]
*   [Get a Free API License][3]

**TIP**

You may want to check out Aspose [FREE macro removal web app][4].

## C# API to Protect Excel VBA Macros {#C-API-to-Protect-Excel-VBA-Macros}

In order to protect the Excel VBA macros, we will use [Aspose.Cells for .NET][5] API. It is a powerful spreadsheet manipulation API that lets you implement Excel automation from within your .NET applications. In addition, the API allows you to work with VBA macros in Excel files seamlessly. You can either [download][6] the API's DLL or install it using [NuGet][7].

```
PM> Install-Package Aspose.Cells
```

## Protect Excel VBA Macros using C# {#Protect-Excel-VBA-Macros-using-C}

VBA macros in Excel spreadsheets are encapsulated by VBA projects where each VBA project may contain one or more VBA macros (or modules). Therefore, to protect the VBA macros, you simply need to apply protection on the VBA project.

The following are the steps of how to protect an Excel VBA project.

*   Load the Excel file using [Workbook][8] class.
*   Access the VBA project into a [VbaProject][9] object using [Workbook.VbaProject][10] property.
*   Protect the VBA project with a password using [VbaProject.Protect(bool, string)][11] method.
*   Save the updated Excel file using [Workbook.Save(String)][12] method.

The following code sample shows how to protect the Excel VBA project using C#.

{{< gist aspose-com-gists 3cf479aa91ba1bc20d9725875b7b656b "protect-vba.cs" >}}

MS Excel shows the following message when you try to view the password-protected VBA project.



{{< figure align=center src="images/Protect-Excel-VBA.jpg" alt="Protect Excel VBA">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][13] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to protect VBA macros in Excel files using C#. The step-by-step guide along with API references and code sample have shown how to apply a password to a VBA project. You can explore more about Aspose.Cells for .NET using the [documentation][14]. In case you would have any queries, feel free to let us know via our [forum][15].

## See Also

*   [Create MS Excel Files in C# without MS Office][16]




[1]: #C-API-to-Protect-Excel-VBA-Macros
[2]: #Protect-Excel-VBA-Macros-using-C
[3]: #Get-a-Free-API-License
[4]: https://products.aspose.app/slides/remove-macros
[5]: https://products.aspose.com/cells/net
[6]: https://downloads.aspose.com/cells/net
[7]: https://nuget.org/packages/Aspose.Cells
[8]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbaproject
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/vbaproject
[11]: https://apireference.aspose.com/cells/net/aspose.cells.vba/vbaproject/methods/protect
[12]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/cells/net/getting-started/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





