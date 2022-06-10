---
title: 'Apply Metered License, Retrieve Spreadsheet''s Fonts List, Auto-Fit Columns and Rows while Importing HTML and Convert Text to Columns with Aspose.Cells for .NET 17.02.0'
date: Fri, 24 Feb 2017 10:23:08 +0000
draft: false
url: /2017/02/24/apply-metered-license-retrieve-spreadsheets-fonts-list-auto-fit-columns-rows-importing-html-convert-text-columns-aspose.cells-.net-17.02.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v17.02.0][2]. The new release includes some valuable features and other enhancements with critical bug fixes. Please see the detailed release notes in order to get an idea about what is new and what has been fixed with this version of Aspose.Cells for .NET. The release notes also list any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET.

## Introducing Metered Licensing

Aspose.Cells for .NET now offers the metered licensing mechanism in parallel to its traditional licensing. In order to provide the usage-based licensing model, Aspose.Cells for .NET has exposed the Metered class that allows the developers to set public and private keys by calling its SetMeteredKey method. The metered licensing system monitors the regular usage of Aspose.Cells API and keep track of the Aspose API licenses.

Following piece of code demonstrates [how to set metered public & private keys and reterieve the consumption logs][3].

```
//Set metered public and private keys
Metered metered = new Metered();
//Access the setMeteredKey property and pass public and private keys as parameters
metered.SetMeteredKey("*************", "*************");
//Instantiate a new Workbook
Workbook workbook = new Workbook();
//Check if the license is set
Console.WriteLine(workbook.IsLicensed);
 
 
//Get the Consumption quantity
decimal amountBefore = Metered.GetConsumptionQuantity();
Console.WriteLine(amountBefore);
Workbook workbook2 = new Workbook("e:\\test2\\Book1.xlsx");
workbook2.Save("e:\\test2\\out1.xlsx");
//Since uploading data is already running on another thread, so you might need to wait for some time (optional)
System.Threading.Thread.Sleep(10000);
//Get the Consumption quantity again which should be greater a bit
decimal amountAfter = Metered.GetConsumptionQuantity();
Console.WriteLine(amountAfter); 
```

## Get List of Fonts Used in Spreadsheet

Aspose.Cells for .NET 17.02.0 has exposed the GetFonts method for the Workbook class. The Workbook.GetFonts method returns the list of individual fonts used to format the cell contents for a given spreadsheet. The list returned by the Workbook.GetFonts method is in the form of an array of type Font. 

The newly exposed method is useful in scenarios where the developers require to extract the list of the fonts used in a particular spreadsheet. The extracted list can further be used to match the available fonts on the machine before rendering the spreadsheet. This is because, if Aspose.Cells APIs are not able to find the required fonts, they try to replace the required font with some other suitable font which is present on the system.

Following code snippet demonstrates the usage of Workbook.GetFonts method in order to [extract the list of fonts used in the sample spreadsheet][4].

```
//Load source workbook
Workbook wb = new Workbook("sampleGetFonts.xlsx");
 
//Get all the fonts inside the workbook
Aspose.Cells.Font[] fnts = wb.GetFonts();
 
//Print all the fonts
for(int i=0; i<fnts.Length; i++)
{
    Debug.WriteLine(fnts[i]);
} 
```

## Auto-Fit Columns and Rows while Importing HTML

Aspose.Cells for .NET has now added the HTMLLoadOptions.AutoFitColsAndRows property which indicates if the API should auto-fit columns and rows while importing the HTML in its object mode. The Boolean type property has the default value as false which means that the cell heights & widths will be imported as they are, however, when the aforementioned property is set to true, the API tries to adjust the column widths and row heights according to the contents.

The following code snippet demonstrates the usage of HTMLLoadOptions.AutoFitColsAndRows property. Please review the detailed article if you wish to get more in-depth knowledge on [how to auto fit cell contents while importing HTML in Aspose.Cells object model][5].

```
// Create an instance of HTMLLoadOptions
HTMLLoadOptions loadOptions = new HTMLLoadOptions();
 
// Set the AutoFitColsAndRows property to true
loadOptions.AutoFitColsAndRows = true;
 
// Create an instance of Workbook and load HTML while passing
// the object of HTMLLoadOptions class created above
Workbook book = new Workbook(dir + "sample.htm", loadOptions); 
```

## Convert Text to Columns

Latest revision of Aspose.Cells for .NET has exposed the Cells.TextToColumns method in order to mimic the Excel's **Text to Columns** feature. Excel provides this feature from the command group **Data Tools** under the **Data** tab. Please note, in order to split the contents of a column to multiple columns, the data should contain a specific delimiter such as a comma (or any other character) based on which the API tries to split the contents of a cell to multiple cells.

The following code snippet demonstrates the simplest usage scenario of Cells.textToColumns method. Please review the detailed article if you wish to get more in-depth knowledge on [how to convert text to columns][6].

```
//Create a workbook.
Workbook wb = new Workbook();
 
//Access first worksheet.
Worksheet ws = wb.Worksheets[0];
 
//Add people name in column A. Fast name and Last name are separated by space.
ws.Cells["A1"].PutValue("John Teal");
ws.Cells["A2"].PutValue("Peter Graham");
ws.Cells["A3"].PutValue("Brady Cortez");
ws.Cells["A4"].PutValue("Mack Nick");
ws.Cells["A5"].PutValue("Hsu Lee");
 
//Create text load options with space as separator.
TxtLoadOptions opts = new TxtLoadOptions();
opts.Separator = ' ';
 
//Split the column A into two columns using TextToColumns() method.
//Now column A will have first name and column B will have second name.
ws.Cells.TextToColumns(0, 0, 5, opts);
 
//Save the workbook in xlsx format.
wb.Save("outputTextToColumns.xlsx"); 
```

## Warning Callback for Template Loading

Aspose.Cells for .NET 17.02.0 has exposed the WarningCallback property for the LoadOptions class in order to get or set the warning callbacks. Developers have to implement the IWarningCallback interface in order to get custom warnings in their applications.

Here is a simple usage scenario of LoadOptions.WarningCallback property to [get warnings when an input spreadsheet contains duplicate named ranges][7].

```
//Implement IWarningCallback interface to catch warnings while loading workbook
private class WarningCallback : IWarningCallback
{
    public void Warning(WarningInfo warningInfo)
    {
        if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
        {
            Console.WriteLine("Duplicate Defined Name Warning: " + warningInfo.Description);
        }
    }
}//WarningCallback
 
//------------------------------------------------------------------
 
//Create load options and set the WarningCallback property 
//to catch warnings while loading workbook
LoadOptions options = new LoadOptions();
options.WarningCallback = new WarningCallback();
             
//Load the source excel file
Workbook book = new Workbook("sampleDuplicateDefinedName.xlsx", options);
 
//Save the workbook 
book.Save("outputDuplicateDefinedName.xlsx"); 
```

## Trim Leading Blank Rows & Columns while Exporting Contents to Text Formats

This revision of Aspose.Cells for .NET has exposed Boolean type TrimLeadingBlankRowAndColumn property for the TxtSaveOptions class that indicates whether leading blank rows and columns should be trimmed like Excel does while exporting data to CSV or Tab-delimited formats. The default value of aforementioned property is false.

In case the data on the worksheet does not start from the first cell, that is: A1, the Excel application removes the leading blank rows and columns while exporting the data to CSV or Tab-delimited formats, however, Aspose.Cells APIs by default, retain the blank rows & columns for the same sample in order to keep the data location retained if the exported CSV or Tab-delimited files have to be imported back using Aspose.Cells APIs.

Here is a simple usage scenario of TxtSaveOptions.TrimLeadingBlankRowAndColumn property. Please check the article on [trimming leading empty cells while storing contents in text formats][8] for more details.

```
//Load source worbook
Workbook wb = new Workbook("sampleTrimBlankColumns.xlsx");
 
//Save in csv format
wb.Save("outputWithoutTrimBlankColumns.csv", SaveFormat.CSV);
 
//Now save again with TrimLeadingBlankRowAndColumn as true
TxtSaveOptions opts = new TxtSaveOptions();
opts.TrimLeadingBlankRowAndColumn = true;
 
//Save in csv format
wb.Save("outputTrimBlankColumns.csv", opts); 
```

## Other Enhancements and Fixes

Aspose.Cells for .NET 17.02.0 has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Support to load Excel 2016 chart types.
*   [Rename duplicate columns automatically while exporting worksheet data][9].
*   [Binding Worksheet to a Customized Collection Object using GridWeb][10].
*   [Split Panes in GridDesktop Worksheet][11].
*   Handled a few exceptions, such as NullReferenceException & ArgumentOutOfRangeException, etc.

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel Excel file formats, rendering shapes, rendering and manipulating charts, rendering HTML to Excel and vice versa, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. The formula calculation engine is also enhanced in the new release.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   The BuiltInDocumentPropertyCollection.RevisionNumber property has been replaced by the BuiltInDocumentPropertyCollection.Revision property.
*   Added Shape.TextShapeType property that gets or sets the preset text shape type from a list of predefined types stored in AutoShapeType enumeration.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Aspose.Cells for .NET Download Section][13].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-17.02.0/
[3]: https://docs.aspose.com/display/cellsnet/Licensing#Licensing-ApplyingMeteredLicense
[4]: https://docs.aspose.com/display/cellsnet/Get+a+List+of+Fonts+used+in+a+Spreadsheet+or+Workbook
[5]: https://docs.aspose.com/display/cellsnet/AutoFit+Columns+and+Rows+while+loading+HTML+in+Workbook
[6]: https://docs.aspose.com/display/cellsnet/Convert+Text+to+Columns+using+Aspose.Cells
[7]: https://docs.aspose.com/display/cellsnet/Get+Warnings+while+Loading+Excel+File
[8]: https://docs.aspose.com/display/cellsnet/Trim+Leading+Blank+Rows+and+Columns+while+exporting+spreadsheets+to+CSV+format
[9]: https://docs.aspose.com/display/cellsnet/Rename+duplicate+columns+automatically+while+exporting+worksheet+data
[10]: https://docs.aspose.com/display/cellsnet/Binding+Worksheet+to+a+Customized+Collection+Object+using+GridWeb
[11]: https://docs.aspose.com/display/cellsnet/Split+Panes+in+GridDesktop+Worksheet
[12]: https://www.aspose.com/products/cells/net
[13]: http://www.aspose.com/downloads/cells/net
[14]: http://www.aspose.com/api/net/cells
[15]: https://forum.aspose.com/
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




