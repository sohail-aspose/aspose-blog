---
title: 'Disable Compatibility Checker in Excel Files using C#'
seoTitle: "Disable Compatibility Checker in Excel Files using C# | .NET Excel Library"
description: "Use .NET Excel library to enable or disable compatibility checker in XLSX/XLS in C# or VB.NET. Turn the MS Excel compatibility mode on/off dynamically."
date: Sun, 10 Oct 2021 15:07:00 +0000
draft: false
url: /2021/10/10/disable-compatibility-checker-in-excel-csharp/
author: Usman Aziz
summary: 'Various versions of MS Excel are available and being used around the world. This makes it possible that the newer versions provide features that may not be available in the older ones. Therefore, MS Excel uses the compatibility checker to degrade the features which are not supported by an older format when saving the files. However, in certain cases, you have to disable the compatibility checker. In this article, you will learn **how to disable the compatibility checker for MS Excel workbooks in C#**.'
tags: ['disable compatibility checker in Excel in csharp', 'disable excel compatibility checker csharp', 'disable xls compatibility checker csharp', 'disable xlsx compatibility checker csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Enable or Disable Excel Compatibility Checker in Java">}}


MS Excel is a widely used spreadsheet application, which is available in different versions. Therefore, compatibility issues may occur when opening a file having the latest features in an older version of MS Excel. MS Excel contains a compatibility checker, which is executed when saving the files. It verifies that newer features, which are not supported by the older formats, are not used in the file. However, in certain cases, you have to disable the compatibility checker. In this article, you will learn **how to disable the compatibility checker for MS Excel workbooks in C#**.

*   [.NET Library for Excel Compatibility Checker][1]
*   [Disable Compatibility Checker in Excel Files][2]

## C# Library to Disable Compatibility Checker in Excel {#Library-for-Excel-Compatibility-Checker}

[Aspose.Cells for .NET][3] is a popular spreadsheet manipulation API that allows you to create spreadsheet files from scratch. Also, it lets you manipulate existing Excel files quite easily. We will use this API to disable the compatibility checker for Excel files. You can [download][4] the API’s DLL or install it using [NuGet][5].

```
PM> Install-Package Aspose.Cells
```

## Disable Compatibility Checker in Excel Files {#Enable-or-Disable-Excel-Compatibility-Checker}

The compatibility checker for an Excel file can be disabled by updating the workbook's settings. The following are the steps to achieve that.

*   First, use [Workbook][6] class to load the desired Excel file.
*   Then, use [Workbook.Settings.CheckCompatibility][7] property to disable the compatibility checker (set true and false to enable and disable checker, respectively).
*   Finally, save Excel file using [Workbook.Save(string)][8] method.

The following code sample shows how to disable the compatibility checker using C#.

{{< gist aspose-com-gists fde0ed041326c57351a5857dcb5b6c50 "disable-excel-compatibility-checker.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][9].

## Conclusion

While manipulating Excel files from within your .NET applications, you may need to disable the compatibility checker. To achieve that, in this article, you have learned how to enable or disable the compatibility checker for Excel files using C#. Apart from that, you can explore other features of Aspose.Cells for .NET using the [documentation][10]. In addition, you can post your questions and queries on our [forum][11].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][12]
*   [Create Excel Files in C# without MS Office][13]




[1]: #Library-for-Excel-Compatibility-Checker
[2]: #Enable-or-Disable-Excel-Compatibility-Checker
[3]: https://products.aspose.com/cells/net/
[4]: https://downloads.aspose.com/cells/net/
[5]: https://www.nuget.org/packages/Aspose.Cells/
[6]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[7]: https://apireference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/checkcompatibility
[8]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/cells/net/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[13]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




