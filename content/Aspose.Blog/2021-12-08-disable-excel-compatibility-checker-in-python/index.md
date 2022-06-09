---
title: 'Disable Compatibility Checker in Excel in Python'
seoTitle: "Disable Compatibility Checker in Excel in Python | Python Excel Lib"
description: "Use Python Excel library to enable or disable compatibility checker in XLSX/XLS in Python. Turn the MS Excel compatibility mode on/off dynamically."
date: Wed, 08 Dec 2021 07:09:54 +0000
draft: false
url: /2021/12/08/disable-excel-compatibility-checker-in-python/
author: Usman Aziz
summary: 'MS Excel compatibility checker ensures that a file in an older format does not use the features provided by the newer Excel version. Thus, people using older versions of Excel do not face compatibility issues. While manipulating Excel files, you may need to disable the compatibility checker dynamically. To achieve it, this article shows **how to enable or disable the compatibility checker for MS Excel workbooks in Python**.'
tags: ['Python library for compatibility checker in Exel', 'disable compatibility checker in Excel in Python', 'enable compatibility checker in Excel in Python', 'python excel library']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Enable or Disable Excel Compatibility Checker in Python">}}


MS Excel compatibility checker ensures that a file in an older format does not use the features provided by the newer Excel version. Thus, people using older versions of Excel do not face compatibility issues. While manipulating Excel files, you may need to disable the compatibility checker dynamically. To achieve it, this article shows **how to disable the compatibility checker for MS Excel workbooks in Python**.

*   [Python Library for Excel Compatibility Checker][1]
*   [Disable Excel Compatibility Checker][2]

## Python Library to Disable Excel Compatibility Checker {#Python-Library-for-Excel-Compatibility-Checker}

[Aspose.Cells for Python via Java][3] is a powerful and feature-rich spreadsheet manipulation API. It provides basic as well as advanced features to create and manipulate MS Excel files. We will use this library to enable or disable the compatibility checker in Excel files. You can either [download][4] the API or install it using the following pip command.

```
> pip install aspose-cells
```

## Disable Excel Compatibility Checker {#Enable-or-Disable-Excel-Compatibility-Checker}

In order to enable or disable the compatibility checker for an Excel workbook, you need to update the workbook's settings. The following are the steps to perform this operation.

*   First, load the Excel file using [Workbook][5] class.
*   Then, disable compatibility checker using [Workbook.getSettings().setCheckCompatibility(boolean)][6] method (set True and False to enable and disable checker, respectively).
*   Finally, save the updated workbook using [Workbook.save(string)][7] method.

The following code sample shows how to disable the compatibility checker using Python.

{{< gist aspose-com-gists 8e93f456ca967bd7c9781069dd22a49b "disable-excel-compatibility-checker.py" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Python via Java without evaluation limitations using a [temporary license][8].

## Conclusion

MS Excel compatibility checker restricts the users to use newer features in an older version of Excel file. In this article, you have seen how to disable compatibility checker in Excel files using Python. Besides, you can also explore other features of Aspose.Cells for Python via Java using the [documentation][9]. In case you would have any queries, you can post on our [forum][10].

## See Also

*   [Encrypt and Decrypt Excel Files in Python][11]
*   [Create MS Excel Files using Python – Python Excel API][12]




[1]: #Python-Library-for-Excel-Compatibility-Checker
[2]: #Enable-or-Disable-Excel-Compatibility-Checker
[3]: https://products.aspose.com/cells/python-java/
[4]: https://downloads.aspose.com/cells/python/
[5]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[6]: https://apireference.aspose.com/cells/python/asposecells.api/workbooksettings#CheckCompatibility
[7]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/cells/pythonjava/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/06/01/encrypt-and-decrypt-excel-files-in-python/
[12]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/




