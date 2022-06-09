---
title: 'Protect and Unprotect Excel Files using C#'
seoTitle: ""
description: ""
date: Mon, 14 Dec 2020 10:12:00 +0000
draft: false
url: /2020/12/14/protect-or-unprotect-excel-files-using-csharp/
author: Usman Aziz
summary: 'MS Excel provides convenient ways of storing and managing small or large amounts of data. Workbooks are widely used to maintain the datasets, analyze the data, perform activities related to finance or human resources, and etc. With the advancement in technology, the ways of getting unauthorized access to data have also been increased. Therefore, MS Excel lets you protect the workbooks using the password. In this article, you will learn **how to automate the spreadsheet protection features and protect or unprotect Excel files programmatically using C#**.'
tags: ['excel protection in csharp', 'protect Excel files in csharp', 'unprotect excel files in csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Protect-Excel-Files-C.jpg" alt="protect unprotect excel files c#">}}


MS Excel provides convenient ways of storing and managing small or large amounts of data. Excel workbooks are widely used to maintain the datasets, analyze the data, perform activities related to finance or human resources, and etc. With the advancement in technology, the ways of getting unauthorized access to data have also been increased. Therefore, MS Excel lets you protect the workbooks using the password. In this article, you will learn **how to automate the spreadsheet protection features and protect and unprotect Excel files programmatically using C#**.

*   [C# API to Protect Excel Files][1]
*   [Protect Excel Files using C#][2]
*   [Unprotect Excel Files using C#][3]

## C# API to Protect Excel Files - Free Download {#API-to-protect-Excel-files}

[Aspose.Cells for .NET][4] is a well-known spreadsheet manipulation API that lets you create and process Excel files from within your .NET applications. The API allows you to protect and unprotect the Excel files within a few lines of code. You can either [download][5] the binaries of the API or get it installed using [NuGet][6].

```
Install-Package Aspose.Cells
```

## Protect Excel Files using C# {#Protect-Excel-Files-using-C}

Protecting MS Excel is as easy as pie and can be done in a few steps. Simply load the Excel file, protect it, and save the protected file. Furthermore, you can specify the [protection type][7] you want to apply, i.e. protect everything, objects or content only, and etc. The following are the steps to protect an Excel file using Aspose.Cells for .NET.

*   Load the Excel file using [Workbook][8] class.
*   Protect the Excel file using [Workbook.Protect(ProtectionType type, String password)][9] method.
*   Save the protected Excel file using [Workbook.Save(String fileName)][10] method.

The following code sample shows how to protect Excel file using C#.

{{< gist aspose-com-gists 8d4da2809d6fd2a87f994b2890a21d98 "protect-excel-files.cs" >}}

## Unprotect Excel Files using C# {#Unprotect-Excel-Files-using-C}

You can also unprotect the Excel files by providing the password to the API. The following are the steps to unprotect a protected Excel file.

*   Load the Excel file using [Workbook][11] class.
*   Unprotect the Excel file using [Workbook.Unprotect(String password)][12] method.
*   Set password to null using [Workbook.Settings.Password][13] property.
*   Save the Excel file using [Workbook.Save(String fileName)][14] method.

The following code sample shows how to unprotect an Excel file using C#.

{{< gist aspose-com-gists 8d4da2809d6fd2a87f994b2890a21d98 "unprotect-excel-files.cs" >}}

## Conclusion

Protection of the data in MS Excel files is an important aspect of the digital world. Therefore, this article presents how to automate the process of protecting or unprotecting Excel files using C#. The step by step guide along with the API references and code samples make you learn how to implement these features in your .NET applications. You can explore more about the API using [documentation][15].

## See Also

*   [Convert MS Excel XLSX Files to DOCX using C#][16]




[1]: #API-to-protect-Excel-files
[2]: #Protect-Excel-Files-using-C
[3]: #Unprotect-Excel-Files-using-C
[4]: https://products.aspose.com/cells/net
[5]: https://downloads.aspose.com/cells/net
[6]: http://nuget.org/packages/Aspose.Cells
[7]: https://apireference.aspose.com/cells/net/aspose.cells/protectiontype
[8]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/methods/protect
[10]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[12]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/methods/unprotect
[13]: https://apireference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/password
[14]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[15]: https://docs.aspose.com/cells/net/developer-guide/
[16]: https://blog.aspose.com/2020/10/15/convert-excel-xlsx-to-docx-using-csharp/





