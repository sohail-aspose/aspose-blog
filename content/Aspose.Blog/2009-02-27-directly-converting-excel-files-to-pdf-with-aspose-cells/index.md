---
title: 'Directly Converting Excel Files to Pdf with Aspose.Cells'
date: Fri, 27 Feb 2009 18:40:00 +0000
draft: false
url: /2009/02/27/directly-converting-excel-files-to-pdf-with-aspose-cells/
author: Laurence
summary: ''
tags: ['Aspose.Cells for .NET', 'Convert Excel to PDF', 'Excel to PDF', 'aspose excel to pdf', 'excel to pdf c#']
categories: ['Aspose.Cells Product Family']
---

In previous versions, converting Excel files to Pdf needs two components: Aspose.Cells and Aspose.Pdf. With the new version v4.7.0, users can use [Aspose.Cells for .NET][1] only to implement this feature. This new change greatly optimizes speed and memory usage.

You will utilize the overloaded **Save** method of the **[Workbook][2]** class providing the **_[SaveFormat.Pdf][3]_** enum member that converts the native excel file to pdf format.

The above steps are implemented in the following example.

**Example:**

\[C#\]

```
// Instantiate the Workbook object
// Open an Excel file
Workbook workbook = new Workbook("Book1.xls");

// Save the document in PDF format
workbook.Save("output.pdf", SaveFormat.Pdf);
```

\[VB.NET\]

```
Dim workbook As Workbook = New Workbook("Book1.xls")
workbook.Save("output.pdf", SaveFormat.Pdf)
```

Please download and try the new version at: 

*   [https://downloads.aspose.com/cells/net][4]




[1]: https://products.aspose.com/cells/net
[2]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[3]: https://apireference.aspose.com/net/cells/aspose.cells/saveformat
[4]: https://downloads.aspose.com/cells/net




