---
title: 'InsightSoftware exports data to Microsoft Excel using Aspose.Cells for .NET'
date: Tue, 28 Jul 2009 04:07:18 +0000
draft: false
url: /2009/07/28/export-of-data-to-microsoft-excel-through-apis/
author: Danny Graham
summary: ''
tags: ['Aspose.Cells', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Insight_Software_Logo.png" alt="">}}


## Product Background / Overview

[INSIGHT][1]® is a real-time productivity tool designed to optimize the customer’s JD Edwards or Oracle eBusinessSuite system for improved business performance. Operations such as real-time reporting, data reconciliation, integrity management and entire process optimization are achieved quickly and easily with this powerful, end-user tool. For example, INSIGHT’s General Ledger module helps users produce their key financial reports and provide continual real-time access to answer all their important financial questions. Accountants are able to close the month-end quicker and business managers are able to gain greater financial insight.

An important feature is the ability to be able to take numbers displayed in the Insight product and allow them to be displayed in Microsoft Excel. This is where [Aspose.Cells for .NET][2] comes in.

## Requirements Scenario

The worksheet generation engine needed to be able to:

*   Handle many thousands of rows of data and do so very quickly.
*   Accurately reflect the cell formatting set up in INSIGHT®.
*   Output many reports to a single Excel Workbook.
*   Support Excel 2003 & Excel 2007.

## Solution Implementation

From a user perspective, we simply use an Export button on the product ribbon. When it is clicked the content is recreated as an xls or xslx file and then opened for viewing in Excel. From a coding perspective, [Aspose.Cells for .NET][3] follows the Microsoft Excel object model very closely, so porting the code of our previous solution to use [Aspose.Cells][4] was straight forward.

## Benefits

The most obvious benefit was a huge boost in performance. [Aspose.Cells][5] can generate very large xls files extremely quickly and using a fairly small memory footprint. In a product that can provide many thousands of rows of data, this is vitally important.

## Conclusion

The [Aspose.Cells for .NET][6] product is extremely fast, reliable, operates in a fairly small memory footprint and from observation seems bug-free – generating large and complex workbooks with consummate ease.

The implementation process was straightforward using the sensibly laid out API.

I wouldn’t hesitate to recommend [Aspose.Cells for .NET][7] to users who require a very high-quality Excel generation solution.



{{< figure align=center src="images/insight-software-aspose-cells-case-study-1024x894.png" alt="" caption="Figure 1: A typical report in INSIGHT® ready to be Exported to Microsoft Excel.">}}




{{< figure align=center src="images/insight-software-aspose-cells-case-study-1-1024x804.png" alt="" caption="Figure 2: Moments later the same data is visible in Microsoft Excel.">}}


**Danny Graham  
**Development Director  
[InsightSoftware.com][8]




[1]: https://insightsoftware.com/
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells/net
[4]: https://products.aspose.com/cells
[5]: https://products.aspose.com/cells
[6]: https://docs.aspose.com/display/cellsnet/Home
[7]: https://products.aspose.com/cells/net
[8]: https://insightsoftware.com/




