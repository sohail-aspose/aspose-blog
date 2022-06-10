---
title: 'Lambodar Inc. resolved Import Data Truncation Issue with Aspose.Cells'
date: Thu, 30 Jul 2009 16:51:22 +0000
draft: false
url: /2009/07/30/solution-for-net-import-data-truncation-issue-using-excel-apis/
author: Shiaw-ling Lai
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## Product Background / Overview



{{< figure align=center src="images/Lambodar-Logo.png" alt="">}}


Lambodar Inc. is a worldwide provider of dynamic software consulting solutions. Founded in 2004, Lambodar offers premium custom software for businesses at cost reducing prices. Armed with a wide arsenal of open-source and proprietary programs at its disposal, Lambodar project managers work intensively to understand the goals and needs of each client to create the perfect software solution. With successful projects in industries such as Finance, Retail, Healthcare, Insurance, Travel, Telecom, and Government, Lambodar has a proven record of the skills and experience for delivering world-class, quality services. Lambodar Inc. is headquartered in Cupertino, California.

In one of its most recent projects, Lambodar needed to simultaneously transfer and upgrade a client’s existing data mining and analysis system from third-party providers to new servers hosted under Lambodar. This project was extremely time-sensitive as there were active projects which needed to be pursued even during the transfer, and demanded high functioning data integration capabilities.

## Requirements Scenario

The data tracking and analysis that the client engaged relied heavily on Microsoft Excel workbook/CSV files. Initially, the proprietary system used an OLEDB (Object Linking and Embedding, Database) provider for the Console Application to read the Excel workbook/CSV file uploaded by users and export it into ADO.NET dataset. Some of the fields from the uploaded workbook data were more than 4,000 thousand characters, but after exporting it into the dataset it was truncated to 255 characters. The data truncation was a major handicap to the system and a critical issue that needed to be resolved, fast.



{{< figure align=center src="images/lambodar-aspose-cells-case-study.png" alt="" caption="Figure 1 - Truncation issue">}}




{{< figure align=center src="images/lambodar-aspose-cells-case-study-1.png" alt="" caption="Figure 2 - Data is truncated in the system without Aspose.Cells">}}


## Solution Implementation

Lambodar had experience with [Aspose products][1] from a previous project creating a medical transcription database. In researching potential fixes, [Aspose.Cells][2] was recommended as a comprehensive solution to the problem.

Using [Aspose.Cells for .NET][3], the system exported data from Excel workbooks using the [ExportDataTable][4] method of the [Cells][5] class. The existing Excel worksheet may contain 500 to 20,000 or more records. To read the rows and columns, the system uses [worksheet.Cells.MaxDataRow][6] and worksheet.Cells.[MaxDataColumn][7], respectively.



{{< figure align=center src="images/lambodar-aspose-cells-case-study-2.png" alt="" caption="Figure 3 - With Aspose.Cells, the data truncation problem is resolved">}}


## Benefits

Implementing Aspose resolved the issues in three key ways:

*   It removed the necessity of installing Microsoft Excel on the server on which the required application is running.
*   It has eliminated the data truncation issue that the system was facing.
*   [Aspose.Cell][8]s has proven to be an excellent tool for exporting the CSV file into a data table.

## Future Implementations

The feature-rich components of Aspose.Cells proved to offer more than just basic data export. Using Aspose greatly expanded the abilities of the client’s proprietary application, and further exploration of its capabilities is definitely in the works for other Lambodar clients.

## Conclusion

[Aspose.Cells][9] resolved the issue of data truncation without requiring any major modification to the existing code. [Aspose.Cells][10] was easy to understand and easy to integrate with the application by adding just a few new lines of code. More extensive workarounds would certainly have been possible, but these would have lacked the simplicity and elegance of the single [Aspose.Cells component solution][11].

**Shiaw-Ling Lai  
**Lambodar Inc.




[1]: https://products.aspose.com/
[2]: https://products.aspose.com/cells
[3]: https://products.aspose.com/cells/net
[4]: https://apireference.aspose.com/net/cells/aspose.cells/cells/methods/exportdatatable/index
[5]: https://apireference.aspose.com/net/cells/aspose.cells/cells
[6]: https://apireference.aspose.com/net/cells/aspose.cells/cells/properties/maxdatarow
[7]: https://apireference.aspose.com/net/cells/aspose.cells/cells/properties/maxdatacolumn
[8]: https://products.aspose.com/cells/family
[9]: https://products.aspose.com/cells
[10]: https://products.aspose.com/cells
[11]: https://products.aspose.com/cells




