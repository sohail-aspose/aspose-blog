---
title: 'Compute Microsoft Excel Selected Color for ColorScale Conditional Formatting using C#'
date: Fri, 22 Nov 2013 11:41:59 +0000
draft: false
url: /2013/11/22/compute-selected-color-for-colorscale-conditional-formatting-in-excel/
author: Amjad Sahi
summary: ''
tags: ['Apply ColorScale Conditional Formatting', 'Excel Files Encryption', 'advanced conditional formatting', 'export Excel workbooks to PDF', 'generate password protected Excel files', 'improved OOXML API', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts', 'select range of cells', 'web based grid control']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


[Aspose.Cells for .NET][1] 7.6.1 has been released. This new release supports calculating the color selected by Microsoft Excel when a ColorScale conditional formatting is used in a template file. Moreover, we have enhanced how the product handles encrypted files so that these do not raise FIPS validation errors now. We have also added some significant improvements for the generated password protected files (by Aspose.Cells), so OOXML API does not raise an exception when loading/opening the files in it. Please see the sample code on how to compute the color selected by Microsoft Excel for ColorScale conditional formatting:

## Sample Code```
//Instantiate a workbook object
//Open the template file
Workbook workbook = new Workbook(@"e:\test2\Book1.xlsx");

//Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Get the A1 cell
Cell a1 = worksheet.Cells["A1"];

//Get the conditional formatting resultant object
ConditionalFormattingResult cfr1 = a1.GetConditionalFormattingResult();

//Get the ColorScale resultant color object
Color c = cfr1.ColorScaleResult;

//Read the color
Console.WriteLine(c.ToArgb().ToString());
Console.WriteLine(c.Name); 
```

## Several New Fixes

We have fixed an exception when rendering images from Excel worksheets.

In this release, several important issues have been addressed. For example, issues around rendering Microsoft Excel file formats, rendering and manipulating PivotTables, rendering images from Excel worksheets, manipulating custom document properties, working with advanced conditional formatting (Microsoft Excel 2007/2010), rendering and manipulating Charts, rendering images files from Charts and exporting Excel workbooks to PDF format have been resolved. A few improvements are also made pertaining to the formula calculation engine of Aspose.Cells for .NET.

We have made a few enhancements regarding navigation between worksheets in the web based grid control provided by Aspose.Cells for .NET. Now, you can select a range of cells and delete the cells and data in one go. We also fixed an issue regarding CellImage object in GridWeb.

To see a complete list of enhancements and fixes and to download Aspose.Cells for .NET 7.6.1, please visit the [download page][2].




[1]: https://products.aspose.com/cells/net
[2]: https://downloads.aspose.com/cells/net




