---
title: 'Get Font Substitution Warnings when Rendering Spreadsheets with Aspose.Cells for .NET 8.1.2'
date: Mon, 04 Aug 2014 11:17:07 +0000
draft: false
url: /2014/08/04/get-font-substitution-warnings-while-rendering-spreadsheets-with-aspose.cells-for-.net-8.1.2-2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png)Aspose.Cells for .NET 8.1.2 has been released. This release contains some useful features and improvements.  It also includes over 20 fixes and other enhancements. However, if you are planning to upgrade your project to use the latest build, we recommend you to check the Public API Changes section first. Below, we list some major features and other enhancements in this month’s release.

## Getting Warnings for Font Substitution

The Aspose.Cells APIs generally uses TrueType Fonts (TTFs) when a task involves rendering spreadsheets to images or portable formats such as PDF. Aspose.Cells detects which fonts are required by scanning the spreadsheet styles and then tries to find the required fonts on the machine where the conversion is taking place. There could be situations when the required fonts are not available. In such cases, Aspose.Cells substitutes the required font with a similar available one.

With this release, Aspose.Cells provides the means to receive warnings if a font substitution has occurred during the spreadsheet rendering process. This mechanism is available through a set of classes, interfaces and properties that have been added with version 8.1.2.

This is how you may use the latest API to Get Warnings for Font Substitution:

```
public class WarningCallback : IWarningCallback
{
    public void Warning(WarningInfo info)
    {
        if (info.WarningType == WarningType.FontSubstitution)
        {
            Debug.WriteLine("WARNING INFO: " + info.Description);
        }
    }
}

//........
//........

void Run()
{
    Workbook workbook = new Workbook("source.xlsx");

    PdfSaveOptions options = new PdfSaveOptions();
    options.WarningCallback=new WarningCallback();

    workbook.Save("output.pdf", options);
} 
```

## Other Enhancements and Fixes

In the new version, we have fixed a few exceptions that occurred while writing Microsoft Excel files to PDF and ODS.

In this release, several important issues have been addressed. For example, issues around manipulating style and formatting, rendering and manipulating pivot tables, manipulating shapes, rendering images from Excel worksheets, manipulating charts, rendering images files from charts, Smart Markers and exporting Excel workbooks to PDF format have been resolved. We have also fixed a few issues regarding Aspose.Cells formula calculation engine.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.1.2, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry561399.aspx




