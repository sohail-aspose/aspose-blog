---
title: 'Implement Custom Calculation Engine, Add Custom XML Parts to Spreadsheets and Access TextBox via its Name with Aspose.Cells for .NET 8.7.2'
date: Fri, 01 Apr 2016 11:58:45 +0000
draft: false
url: /2016/04/01/implement-custom-calculation-engine-add-custom-xml-parts-to-spreadsheets-and-access-textbox-via-its-name-with-aspose.cells-for-.net-8.7.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")We are pleased to announce our next version of Aspose.Cells for .NET v8.7.2. This release contains some valuable enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements (of this month's release) here.

## Implement Custom Calculation Engine

Aspose.Cells APIs have powerful calculation engine that can calculate almost all of the Microsoft Excel functions with precision. However, sometimes the application requirement demands to override any Excel formula in order to get desired results, such as return 3 for function **\=SUM(1,1)**, which isn't possible with default Aspose.Cells calculation engine.

The recent revision of Aspose.Cells for .NET allows you to extend the default calculation engine to get desired results. Aspose.Cells for .NET 8.7.2 has exposed two new classes for this purpose as detailed below.

*   AbstractCalculationEngine: Represents custom calculation engine to extend the default calculation engine of Aspose.Cells.
*   CalculationData: Represents the required data when calculating one function, such as function name, parameters and so forth.

By implementing custom calculation engine, users can override for all Excel's native functions with more flexibility. Below provided is the simplest usage scenario to define a custom calculation engine that extends AbstractCalculationEngine in order to override the Excel's default SUM function to get desired results.

```
class CustomEngine : AbstractCalculationEngine
{
    public override void Calculate(CalculationData data)
    {
        if(data.FunctionName.ToUpper()=="SUM")
        {
            double val = (double)data.CalculatedValue;
            val = val + 30;

            data.CalculatedValue = val;
        }

    }
} 
```

Here is how to use the newly defined custom calculation engine to get desired results.

```
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

Cell a1 = sheet.Cells["A1"];
a1.Formula = "=Sum(B1:B2)";

sheet.Cells["B1"].PutValue(10);
sheet.Cells["B2"].PutValue(10);

//Without Custom Engine, the value of cell A1 will be 20
workbook.CalculateFormula();

Console.WriteLine("Without Custom Engine Value of A1: " + a1.StringValue);

//With Custom Engine, the value of cell A1 will be 50
CustomEngine engine = new CustomEngine();

CalculationOptions opts = new CalculationOptions();
opts.CustomEngine = engine;

workbook.CalculateFormula(opts);

Console.WriteLine("With Custom Engine Value of A1: " + a1.StringValue); 
```

## Add Custom XML Parts to Spreadsheets

Custom XML parts are the XML based data files stored by different applications like SharePoint inside the spreadsheet files. This data is consumed by different applications, however, Microsoft Excel application does not make use of this data so there is no GUI to add such data in the spreadsheets. One can view this data by extracting the contents of the spreadsheet (XLSX) using applications such as WinRar, and inspect the contents of the customXml folder.

Aspose.Cells for .NET API provides the ContentTypePropertyCollection.Add which can be used to add Custom XML data to the spreadsheet as demonstrated below.

```
Workbook workbook = new Workbook();
workbook.ContentTypeProperties.Add("BookStore", booksXML);
workbook.Save("output.xlsx"); 
```

## Access TextBox from Collection

Aspose.Cells for .NET 8.7.2 has exposed the overloaded indexer for the TextBoxCollection class in order to access the instance of TextBox using its name as demonstrated below.

```
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

int idx = sheet.TextBoxes.Add(10, 10, 10, 10);

//Create a texbox with some text and assign it some name
TextBox tb1 = sheet.TextBoxes[idx];
tb1.Name = "MyTextBox";
tb1.Text = "This is MyTextBox";

//Access the same textbox via its name
TextBox tb2 = sheet.TextBoxes["MyTextBox"];

//Displaying the text of the textbox accessed by its name
Console.WriteLine(tb2.Text); 
```

## Other Enhancements and Fixes

The most notable other enhancements in this release are as follows:

*   Detect encryption on ODS files.
*   Set the OleObject.ImageData for existing OleObjects in the Workbook.

We have also handled a few exceptions regarding reading/writing MS Excel files, rendering Excel files to TIFF/PDF and calculating Pivot Tables data.

In this release, several important issues have been addressed. For example, issues around manipulating Microsoft Excel file formats, manipulating named ranges, manipulating shapes, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. The Aspose.Cells formula calculation engine is improved in this release.

Moreover, in the new release, we have supported IE10 and IE11 browser types in the web based grid control provided by Aspose.Cells for .NET. We also incorporated new events when filtering rows in GridWeb, so, if you need to get number of filtered rows after the filter has been applied, you may easily do that.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.7.2, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells-family/net/new-releases/aspose.cells-for-.net-8.7.2/




