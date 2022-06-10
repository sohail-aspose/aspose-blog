---
title: 'Retrieve Excel Worksheet Instance from Chart using C#'
date: Tue, 21 Oct 2014 11:52:25 +0000
draft: false
url: /2014/10/21/retrieve-excel-worksheet-instance-from-chart-using-csharp/
author: Amjad Sahi
summary: ''
tags: ['Aspose.Cells for .NET', 'Chart to Image', 'Excel Files', 'Excel to PDF', 'PivotTables', 'Spreadsheet Version', 'Workbook Properties', 'charts', 'spreadsheet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


[Aspose.Cells for .NET][1] 8.2.2 has been released. This release contains useful new features and a number of improvements. It introduces contains over 60 improvements, including the new features listed below. If you are planning to upgrade the API from a previous release, we suggest you check the [Public API Changes][2] section.

## Get Worksheet Instance of the Chart using C#

Before the release of Aspose.Cells for .NET 8.2.2, retrieving the Worksheet instance from the Chart object was not possible. The latest version has made this possible by exposing the Worksheet property for the Chart class. Please check the usage scenario below and the detailed article on [Getting Worksheet of a Chart][3].

```
//Create workbook from sample Excel file
Workbook workbook = new Workbook("Book1.xlsx");

//Access first worksheet of the workbook
Worksheet worksheet = workbook.Worksheets[0];

//Print worksheet name
Console.WriteLine("Sheet Name: " + worksheet.Name);

//Access the first chart inside this worksheet
Chart chart = worksheet.Charts[0];

//Access the chart's sheet and display its name again
Console.WriteLine("Chart's Sheet Name: " + chart.Worksheet.Name);
```

## Get a Spreadsheet's Application Version using C#

Microsoft Excel application allows the user to save spreadsheets to different formats corresponding to the application versions such as Microsoft Excel version 2003, 2007, 2010 and 2013. This information is embedded in the spreadsheet, and can be used for version identification. Aspose.Cells for .NET now provides the means to get and set this information with the BuiltInDocumentPropertyCollection.Version property. Check the detailed article on [Getting the Version Number of the Application that Created the Excel Document][4].

## Other Enhancements and Fixes

In the new version, we have fixed a few exceptions that occurred while opening Microsoft Excel 2007/2010 file formats and converting Excel files to PDF format. We have also enhanced the Excel to PDF conversion process which seemed to hang for spreadsheets with millions of rows.

We have also fixed a few issues in the web-based Grid control regarding the paging and formatting features provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.2.2, please visit the [download page][5].




[1]: https://products.aspose.com/cells/net
[2]: https://docs.aspose.com/cells/net/migrating-from-earlier-versions-of-aspose-cells/
[3]: https://docs.aspose.com/cells/net/get-worksheet-of-the-chart/
[4]: https://docs.aspose.com/cells/net/get-the-version-number-of-the-application-that-created-the-excel-document/
[5]: https://downloads.aspose.com/cells/net




