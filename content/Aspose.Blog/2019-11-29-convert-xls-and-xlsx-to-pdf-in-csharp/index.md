---
title: 'Convert Excel XLS and XLSX to PDF in C#'
date: Fri, 29 Nov 2019 11:10:38 +0000
draft: false
url: /2019/11/29/convert-xls-and-xlsx-to-pdf-in-csharp/
author: Muhammad Ahmad
summary: ''
tags: ['Convert Excel Files', 'Convert Excel to PDF', 'XLS to PDF', 'XLS to PDF C#', 'XLSX to PDF', 'XLSX to PDF C#', 'c# excel to pdf', 'c# xlsx to pdf', 'excel to pdf c#']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Excel to PDF C#">}}


This article demonstrates how to convert **Excel** (XLS, XLSX) files to **PDF** format using **C#**. The **Portable Document Format** (**PDF**) format developed by Adobe is used as a standard by many organizations to share and store documents. Exporting documents to PDF is a common scenario for many applications.

*   [C# API for Excel to PDF Conversion][1]
*   [Convert Excel to PDF in C#][2]
*   [Set PDF Compliance in Excel to PDF][3]
*   [Track Excel to PDF Conversion in C#][4]

## C# API for Excel to PDF Conversion {#C#-API-for-Excel-to-PDF-Conversion}

[Aspose.Cells for .NET][5] API makes converting Excel spreadsheets to PDF a breeze. You can either [download][6] the API's DLL or install it using NuGet.

```
PM> Install-Package Aspose.Cells
```

## Convert Excel XLS or XLSX to PDF in C# {#Convert-Excel-to-PDF-in-C#}

[Aspose.Cells for .NET][7] provides easy to use API with which you can convert Excel files to PDF with these simple steps.

1.  Instantiate the [Workbook][8] class with the Excel document that you want to convert.
2.  Save the document in PDF format by specifying the save format as PDF by using the [SaveFormat][9] Enumeration

The following code snippet demonstrates how to convert Excel XLS to PDF in C#.

```
// Instantiate the Workbook object with the Excel file
Workbook workbook = new Workbook("SampleExcel.xls");

// Save the document in PDF format
workbook.Save("outputPDF.pdf", SaveFormat.Pdf);
```

## Convert Excel to PDF/A Compliant PDF using C# {#Set-PDF-Compliance-in-Excel-to-PDF}

PDF/A is an ISO-standardized version of PDF that prohibits features that are not suitable for long term archiving. Saving PDF like this ensures that nothing will break in the long run.

The following code snippet demonstrates this feature by creating a new workbook and convert it to a PDF/A compliant PDF format:

```
// Instantiate new workbook
Workbook workbook = new Workbook();

// Insert a value into the cell A1
workbook.Worksheets[0].Cells[0, 0].PutValue("Testing PDF/A");

// Define PdfSaveOptions
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

// Set the compliance type
pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;

// Save the file
workbook.Save(dataDir + "output.pdf", pdfSaveOptions);
```

## Track Excel to PDF Conversion in C# {#Track-Excel-to-PDF-Conversion-in-C#}

Aspose.Cells for .NET provides the ability to track the conversion progress by providing the [IPageSavingCallback][10] interface. You can create a custom class that implements this interface and assign its instance to [PdfSaveOptions.PageSavingCallback][11] property.

The following code snippet demonstrates how to track the Excel to PDF conversion progress using C#.

```
//load the workbook
Workbook workbook = new Workbook("PagesBook1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//assign the custom class that implements IPageSavingCallback interface
pdfSaveOptions.PageSavingCallback = new TestPageSavingCallback();

workbook.Save("DocumentConversionProgress.pdf", pdfSaveOptions);
```

The following is the custom class that implements the [IPageSavingCallback][12] interface for tracking the conversion process.

```
public class TestPageSavingCallback : IPageSavingCallback
{
    public void PageStartSaving(PageStartSavingArgs args)
    {
        Console.WriteLine("Start saving page index {0} of pages {1}", args.PageIndex, args.PageCount);

        //pages before page index 2 are not rendered.
        if (args.PageIndex < 2)
        {
            args.IsToOutput = false;
        }
    }

    public void PageEndSaving(PageEndSavingArgs args)
    {
        Console.WriteLine("End saving page index {0} of pages {1}", args.PageIndex, args.PageCount);

        //pages after page index 8 are not rendered.
        if (args.PageIndex >= 8)
        {
            args.HasMorePages = false;
        }
    }
}
```

## Conclusion

In this article, you have learned how to convert Excel XLSX or XLS files to PDF using C#. For more information on converting Excel files to PDF, head on over to our documentation, [Convert Excel Workbook to PDF][13]. In case you would have any queries, feel free to let us know via our [forum][14].

## See Also

*   [Create Excel Files in C# without MS Office][15]




[1]: #C#-API-for-Excel-to-PDF-Conversion
[2]: #Convert-Excel-to-PDF-in-C#
[3]: #Set-PDF-Compliance-in-Excel-to-PDF
[4]: #Track-Excel-to-PDF-Conversion-in-C#
[5]: https://products.aspose.com/cells/net
[6]: https://downloads.aspose.com/cells/net
[7]: https://docs.aspose.com/display/cellsnet/Home
[8]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[9]: https://apireference.aspose.com/net/cells/aspose.cells/saveformat
[10]: https://apireference.aspose.com/net/cells/aspose.cells.rendering/ipagesavingcallback
[11]: https://apireference.aspose.com/net/cells/aspose.cells/pdfsaveoptions/properties/pagesavingcallback
[12]: https://apireference.aspose.com/net/cells/aspose.cells.rendering/ipagesavingcallback
[13]: https://docs.aspose.com/cells/net/convert-excel-workbook-to-pdf/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




