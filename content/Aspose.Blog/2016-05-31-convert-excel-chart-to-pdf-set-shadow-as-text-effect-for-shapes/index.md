---
title: 'C#: Convert Chart to PDF and Set Shadow as Text Effect for Shapes in Excel'
date: Tue, 31 May 2016 18:26:49 +0000
draft: false
url: /2016/05/31/convert-excel-chart-to-pdf-set-shadow-as-text-effect-for-shapes/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v8.8.1][1]. The release contains some valuable features along with critical bug fixes and other enhancements. Please see the [release notes][2] in order to get an idea on what is new and what has been fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][3] section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Filter the Data Type while Loading

As per default behavior, Aspose.Cells APIs load everything from the template file into its document object model, providing access to every aspect of the spreadsheet. There could be a scenario where the user does not want to load everything but specific objects, such as charts or shapes. This can be achieved using the newly exposed LoadDataFilterOptions enumeration and LoadOptions.LoadDataFilterOptions property.

Aspose.Cells APIs have added the enumeration LoadDataFilterOptions which can be used to make the selection of data type to be loaded from the template file. Filtering data at the time of loading can improve the performance tremendously, especially when used with LightCells APIs. There are several selections that a user can make in order to customize the loading process by specifying the appropriate value from LoadDataFilterOptions.

The LoadDataFilterOptions enumeration provides the following selections.

1.  All to load everything from the spreadsheet.
2.  None to load nothing from the spreadsheet.
3.  CellBlank loads the cells whose values are blank.
4.  CellBool loads cells whose values are Boolean.
5.  CellData loads cells data including values, formulas and formatting.
6.  CellError loads cells whose values are error.
7.  CellNumeric loads cells whose values are numeric (including Date & Time).
8.  CellString loads cells whose values are text/string.
9.  CellValue loads only cell values (all types).
10.  Chart loads only charts.
11.  ConditionalFormatting loads only conditional formatting rules.
12.  DataValidation loads only data validation rules.
13.  DocumentProperties loads only document properties.
14.  Formula loads formulas including defined names.
15.  MergedArea loads only merged cells.
16.  PivotTable loads Pivot Tables.
17.  Settings loads only Workbook & Worksheet settings.
18.  Shape loads only shapes.
19.  Style loads cells formatting.
20.  Table loads Excel tables/List Objects.

Here is the simple usage scenario to demonstrate the [data filtering at the time of template loading][4].

```
//Set the load options, we only want to load shapes and do not want to load data
LoadOptions opts = new LoadOptions(LoadFormat.Xlsx);
opts.LoadDataFilterOptions = LoadDataFilterOptions.Shape;

//Create workbook object from sample excel file using load options
Workbook wb = new Workbook("sample.xlsx", opts);

//Save the output in pdf format
wb.Save("output.pdf", SaveFormat.Pdf); 
```

## Convert Chart to PDF

Aspose.Cells APIs have already provided the facility to render charts to PDF while using the Chart.ToPdf method. With this release, the API has exposed another overloaded version of the said method that could accept an instance of Stream, allowing the users to save the chart's PDF into streams.

The following code snippet [converts a chart to PDF in memory][5].

```
//Create an instance of Workbook and load an existing spreadsheet with a chart
var workbook = new Workbook(filePath);

//Access first worksheet containing a chart
var worksheet = workbook.Worksheets[0];

//Access first chart from the worksheet
var chart = worksheet.Charts[0];

//Save the chart to PDF as Stream
using (MemoryStream stream = new MemoryStream())
{
    chart.ToPdf(stream);
} 
```

## Setting Shadow as Text Effect for Shapes

Aspose.Cells for .NET 8.8.1 provides the ability to set the shadow as text effects for any shape such as TextBox. The said feature has been provided by exposing the Shape.TextBody property. This property presents the settings of the shape's text and returns FontSetting objects which in turn can be used to set the shadow via ShadowEffect.PresetType property.

Here is the simple usage scenario demonstrating [how to set the shadow effect for the text in a TextBox][6].

```
//Create an instance of Workbook
var book = new Workbook();

//Access first worksheet of the Workbook
var sheet = book.Worksheets[0];

//Add a TextBox to the ShapeCollection
var textBox = sheet.Shapes.AddTextBox(2, 0, 2, 0, 100, 400);

//Set the text of the TextBox
textBox.Text = "This text has the following settings.\n\nText Effects > Shadow > Offset Bottom";

//Set shadow effect for text
for (int i = 0; i < textBox.TextBody.Count; i++)
{
    textBox.TextBody[i].ShapeFont.FillFormat.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
} 
```

## Create Data Validation for GridCell

Aspose.Cells.GridWeb 8.8.1 has exposed the GridCell.CreateValidation & GridCell.RemoveValidation methods to add and remove data validation from the GridCell. Please note, the Aspose.Cells.GridWeb also provides the facility to add data validation rules while using the ValidationCollection.Add method, however, this approach requires to specify the cell range on which data validation rule has to be applied. If the requirement is to specify the data validation rule for just one cell then the GridCell.CreateValidation method can be used without specifying the cell range.

Here is the simple usage scenario of GridCell.CreateValidation method to [add a data validation rule to single GridCell][7].

```
//Access first worksheet
GridWorksheet sheet = GridWeb1.WorkSheets[0];

//Access cell B3
GridCell cell = sheet.Cells["B3"];

//Add validation inside the GridCell
//Any value which is not between 20 and 40 will cause error in a GridCell
GridValidation val = cell.CreateValidation(GridValidationType.WholeNumber, true);
val.Formula1 = "=20";
val.Formula2 = "=40";
val.Operator = GridOperatorType.Between;
val.ShowError = true;
val.ShowInput = true;
```

Similarly, if the requirement is remove the data validation rule from a single GridCell then it's RemoveValidation method can be used to achieve the goal.

## Other Enhancements and Fixes

The most notable enhancements in this release are as follow:

*   Ability to [read data validations from Excel file using Aspose.Cells.GridDesktop][8].
*   Ability to [directly calculate the custom functions without inserting the function in worksheet][9].
*   Ability to [export DataBar, ColorScale and IconSet of conditional formatting to HTML format][10].

We have also handled a few exceptions regarding reading/writing MS Excel files.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Aspose.Cells for .NET Download Section][12].
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-8.8.1/
[2]: http://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+8.8.1+Release+Notes
[3]: http://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: http://docs.aspose.com/display/cellsnet/Filtering+the+kind+of+data+while+loading+the+workbook+from+template+file
[5]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[6]: http://docs.aspose.com/display/cellsnet/Setting+Shadow+of+Text+Effects+of+Shape+or+TextBox
[7]: https://docs.aspose.com/display/cellsnet/Working+with+GridWeb
[8]: http://docs.aspose.com/display/cellsnet/Reading+Data+Validations+in+Excel+file+using+Aspose.Cells.GridDesktop
[9]: http://docs.aspose.com/display/cellsnet/Direct+calculation+of+custom+function+without+writing+it+in+a+worksheet
[10]: http://docs.aspose.com/display/cellsnet/Export+DataBar%2C+ColorScale+and+IconSet+Conditional+Formatting+while+Excel+to+HTML+Conversion
[11]: http://www.aspose.com/.net/excel-component.aspx
[12]: http://www.aspose.com/downloads/cells/net
[13]: http://docs.aspose.com/display/cellsnet/home
[14]: http://www.aspose.com/api/net/cells
[15]: https://forum.aspose.com/
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




