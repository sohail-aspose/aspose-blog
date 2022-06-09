---
title: 'Add Watermark to Excel Worksheets in Python'
seoTitle: "Add Watermark to Excel Worksheet in Python | Aspose.Cells"
description: "Use Python Excel API to add watermark to the Excel files using Python. Source code to define the desired locking properties for watermark in Excel."
date: Fri, 07 May 2021 05:31:00 +0000
draft: false
url: /2021/05/07/add-watermark-to-excel-worksheets-in-python/
author: Usman Aziz
summary: 'Watermarking is one of the common ways of protecting documents from unauthorized usage. More often, a watermark defines the ownership of the copyrighted content. In accordance with that, this article covers how to perform watermarking in Excel files programmatically. Particularly, you will learn **how to add watermark to an Excel worksheet using Python**.'
tags: ['Add a Watermark to Excel Worksheet in Python', 'Python API to Add Watermarks to Excel Files', 'Python Excel API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Excel-Sheets.jpg" alt="Add Watermark to Excel Worksheet Python">}}


Watermarking is one of the common ways of protecting documents from unauthorized usage. More often, a watermark defines the ownership of the copyrighted content. In accordance with that, this article covers how to perform watermarking in Excel files programmatically. Particularly, you will learn **how to add watermark to an Excel worksheet using Python**.

*   [Python API to Add Watermarks to Excel Worksheets][1]
*   [Add a Watermark to Excel Worksheet][2]

## Python API to Add Watermarks to Excel Worksheets {#API-to-Add-Watermarks-to-Excel-Files}

[Aspose.Cells for Python via Java][3] is a spreadsheet manipulation API that lets you create, modify or convert Excel files. We will use it to add watermark to the Excel worksheets. You can [download][4] the API or install it using the following pip command.

*   `pip install aspose-cells`

## Add a Watermark to Excel Worksheet in Python {#Add-a-Watermark-to-Excel-Worksheet}

The following are the steps to add a watermark in an Excel worksheet using Python.

*   First, load the Excel file using [Workbook][5] class by providing its path.
*   Get reference of the [Worksheet][6] to which you want to add the watermark.
*   Create a watermark by adding a new [Shape][7] to the worksheet and set the its text and properties.
*   Set [Shape.setLocked(boolean)][8] property to true to lock the watermark.
*   Set other lock types using [Shape.setLockedProperty(ShapeLockType, boolean)][9] method.
*   Finally, save the updated Excel file using [Workbook.save(String)][10] method.

The following code sample shows how to add a watermark to an Excel worksheet.

{{< gist aspose-com-gists de4eea7fb32397a49be53e5c07aff4f8 "add-watermark-to-Excel.py" >}}

### Output

The following is the screenshot of the Excel worksheet after adding the watermark.



{{< figure align=center src="images/Add-Watermark-to-Excel-Worksheet.jpg" alt="Adding Watermark in Excel Worksheet">}}


## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Python via Java without evaluation limitations using a [temporary license][11].

## Conclusion

Watermarks are extensively used to prevent the illegal usage of copyrighted Excel files. Accordingly, in this article, you have learned how to add watermark to Excel worksheets using Python. You can also explore other features of Aspose.Cells for Python via Java using the [documentation][12]. In case you would have any queries, you can post on our [forum][13].

## See Also

*   [Encrypt and Decrypt Excel Files in Python][14]
*   [Create MS Excel Files using Python – Python Excel API][15]




[1]: #API-to-Add-Watermarks-to-Excel-Files
[2]: #Add-a-Watermark-to-Excel-Worksheet
[3]: https://products.aspose.com/cells/python-java/
[4]: https://downloads.aspose.com/cells/python
[5]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[6]: https://apireference.aspose.com/cells/python/asposecells.api/Worksheet
[7]: https://apireference.aspose.com/cells/python/asposecells.api/Shape
[8]: https://apireference.aspose.com/cells/python/asposecells.api/shape#IsLocked
[9]: https://apireference.aspose.com/cells/python/asposecells.api/shape#setLockedProperty(int,%20boolean)
[10]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/cells/pythonjava
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/06/01/encrypt-and-decrypt-excel-files-in-python/
[15]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





