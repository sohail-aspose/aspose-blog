---
title: 'Gain Theory implemented Excel export capabilities including charts and tables using Aspose.Cells for .NET'
date: Mon, 17 Mar 2008 12:29:41 +0000
draft: false
url: /2008/03/17/complete-excel-export-capabilities-using-apis/
author: Robert Chilvers
summary: ''
tags: ['.NET best component for data export from Excel', 'Aspose.Cells', 'Excel Data export using Aspose.Cells for .NET', 'Export Chart data using Aspose.Cells for .NET', 'Success Stories']
categories: ['Aspose.Cells Product Family']
---

## About GAIN THEORY



{{< figure align=center src="images/gt-logo-green@2x.png" alt="Gain Theory main logo">}}


[Gain Theory][1] fuses data, analytics, technology solutions, and consumer insight capabilities to give marketing and insight professionals the confidence to make smarter, faster business decisions.

The Report Canvas Component is one of the leading products which allows the user to create visual reports based on a pre-loaded dataset. The user can add different components to their canvas including pictures, text boxes, charts, and tables, they then specify the data and how it should be aggregated. The user can then rearrange and resize the objects to fit their page. The user can specify color palettes and save off templates for future use. [Aspose.Cells for .NET][2] was used to export all the objects on the canvas to Excel with the correct data. The component was initially written with VB.Net in Visual Studio 2008.

## Requirements Scenario

We selected Aspose.Cells because of its almost complete Excel export capabilities. Most importantly for us was its ability to export charts and tables especially in Microsoft Excel 2007 – which were lacking in other 3rd party components.

## Solution Implementation

Each object on the report canvas has a function that takes an instance of the [Aspose.Cells for .NET][3] worksheet and adds itself to the worksheet. When the user requests an export the workbook and worksheets are initialized and each object on the report canvas has this function called.

## Benefits

[Aspose.Cells for .NET][4] allowed us to build up the Excel workbook entirely independently of Excel and then save the workbook in the format selected by the user. This saved hours of debugging the interaction when using the Excel interop and implementing different routines for saving to varying versions of Excel.

## Future Implementations

We are likely to use [Aspose.Cells for. NET][5] for all loading and saving of Excel files. This will include loading data templates and exporting results.

## Conclusion

As yet, we have had no problems using the [Aspose.Cells for .NET][6] components and the component has saved us development time in both the short and long-term. Support and Sales queries have been answered swiftly and helpfully. The user produces their canvas, selecting the Export button to save the canvas to Excel using [Aspose.Cells for .NET][7].



{{< figure align=center src="images/ohal-case-study-aspose-cells.png" alt="Report Canvas Component data export using Aspose.Cells for .NET" caption="The user produces their canvas, selecting the Export button to save the canvas to Excel using Aspose.Cells.">}}


**Robert Chilvers  
**Report Canvas Component  
[www.gaintheory.com/][8]




[1]: https://www.gaintheory.com/
[2]: https://products.aspose.com/cells/net
[3]: https://products.aspose.com/cells/net
[4]: https://products.aspose.com/cells/net
[5]: https://products.aspose.com/cells/net
[6]: https://products.aspose.com/cells/net
[7]: https://products.aspose.com/cells/net
[8]: https://www.gaintheory.com/




