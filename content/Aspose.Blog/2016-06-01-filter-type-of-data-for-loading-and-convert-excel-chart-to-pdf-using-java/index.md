---
title: 'Filter Type of Data for Loading and Convert Excel Chart to PDF using Java'
date: Wed, 01 Jun 2016 06:13:29 +0000
draft: false
url: /2016/06/01/filter-type-of-data-for-loading-and-convert-excel-chart-to-pdf-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Convert Chart to PDF', 'Custom Buttons', 'Custom Calculation Engine', 'Data Validation', 'Excel Component', 'Export to HTML', 'Filter Data Loading', 'JSP Grid', 'Java Excel Component', 'Shadow Effect', 'Web Grid', 'conditional formatting']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 8.8.1][1]. This month’s release includes new features, enhancements and bug fixes that further improve the overall stability and usability of the API. Please check the release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Filter the Data Type for Loading

As per default behaviour, Aspose.Cells APIs load everything from the template file into its own object model, providing access to every aspect of the spreadsheet. There could be scenarios where the user does not want to load everything but specific objects, such as charts or shapes. This can be achieved using the newly exposed LoadDataFilterOptions enumeration and LoadOptions.LoadDataFilterOptions property.

Aspose.Cells APIs have added the enumeration LoadDataFilterOptions which can be used to make the selection of data type to be loaded from the template file. Filtering data at the time of loading can improve the performance tremendously, especially when used with LightCells APIs. There are several selections that a user can make in order to customize the loading process by specifying the appropriate value from LoadDataFilterOptions.

The LoadDataFilterOptions enumeration provides the following selections.

1.  ALL to load everything from the spreadsheet.
2.  NONE to load nothing from the spreadsheet.
3.  CELL\_BLANK loads the cells whose values are blank.
4.  CELL\_BOOL loads cells whose values are Boolean.
5.  CELL\_DATA loads cells data including values, formulas and formatting.
6.  CELL\_ERROR loads cells whose values are error.
7.  CELL\_NUMERIC loads cells whose values are numeric (including Date & Time).
8.  CELL\_STRING loads cells whose values are text/string.
9.  CELL\_VALUE loads only cell values (all types).
10.  CHART loads only charts.
11.  CONDITIONAL\_FORMATTING loads only conditional formatting rules.
12.  DATA\_VALIDATION loads only data validation rules.
13.  DOCUMENT\_PROPERTIES loads only document properties.
14.  FORMULA loads formulas including defined names.
15.  MERGED\_AREA loads only merged cells.
16.  PIVOT\_TABLE loads Pivot Tables.
17.  SETTINGS loads only Workbook & Worksheet settings.
18.  SHAPE loads only shapes.
19.  STYLE loads cells formatting.
20.  TABLE loads Excel tables/List Objects.

Here is the simple usage scenario to demonstrate the data filtering at the time of template loading.

```
//Create an instance of LoadOptions & initialize it with type of template to be loaded
LoadOptions options = new LoadOptions(LoadFormat.XLSX);

//Set LoadDataFilterOptions to load only shapes
options.setLoadDataFilterOptions(LoadDataFilterOptions.SHAPE);

//Create an instance of Workbook from a existing spreadsheet using instance of LoadOptions
Workbook book = new Workbook(filePath, options);
```

## Convert Chart to PDF using Java

Aspose.Cells APIs have already provided the facility to render charts to PDF while using the Chart.toPdf method. With this release, the API has exposed another overloaded version of the said method that could accept an instance of OutputStream, allowing the users to save the chart's PDF in an instance of ByteArrayOutputStream.

Following code snippet converts a chart to PDF in memory.

```
//Create an instance of Workbook and load an existing spreadsheet with a chart
Workbook workbook = new Workbook(filePath);

//Access first worksheet containing a chart
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access first chart from the worksheet
Chart chart = worksheet.getCharts().get(0);

//Save the chart to PDF as Stream
ByteArrayOutputStream outStream = new ByteArrayOutputStream();
chart.toPdf(outStream);
```

## Setting Shadow as Text Effect for Shapes

Aspose.Cells for Java 8.8.1 provides the ability to set the shadow as text effects for any shape such as TextBox. The said feature has been provided by exposing the Shape.TextBody property. This property presents the settings of the shape's text and returns FontSetting objects which in turn can be used to set the shadow via ShadowEffect.PresetType property.

Here is the simple usage scenario demonstrating how to set the shadow effect for the text in a TextBox.

```
//Create an instance of Workbook
Workbook book = new Workbook();

//Access first worksheet of the Workbook
Worksheet sheet = book.getWorksheets().get(0);

//Add a TextBox to the ShapeCollection
int index = sheet.getTextBoxes().add(2, 2, 100, 400);
TextBox textBox = sheet.getTextBoxes().get(index);

//Set the text of the TextBox
textBox.setText("This text has the following settings.\n\nText Effects > Shadow > Offset Bottom");

//Set shadow effect for text
for (int i = 0; i < textBox.getTextBody().getCount(); i++)
{
  textBox.getTextBody().get(i).getShapeFont().getFillFormat().getShadowEffect().setPresetType(PresetShadowType.OFFSET_BOTTOM);
}
```

## Create Data Validation for GridCell

Aspose.Cells.GridWeb for Java 8.8.1 has exposed the GridCell.createValidation & GridCell.removeValidation methods to add and remove the data validation from the GridCell. Please note, the Aspose.Cells.GridWeb also provides the facility to add data validation rules while using the ValidationCollection.add method, however, this approach requires to specify the cell range on which data validation rule has to be applied. If the requirement is to specify the data validation rule for just one cell then the GridCell.createValidation method can be used without specifying the cell range.

Here is the simple usage scenario of GridCell.createValidation method to add a data validation rule to single GridCell.

```
//Access first worksheet
GridWorksheet sheet = gridweb.getWorkSheets().get(0);

//Access cell B3
GridCell cell = sheet.getCells().get("B3");

//Add validation inside the GridCell
//Any value which is not between 20 and 40 will cause error in a GridCell
GridValidation val = cell.createValidation(GridValidationType.WHOLE_NUMBER, true);
val.setFormula1("=20");
val.setFormula2("=40");
val.setOperator(OperatorType.BETWEEN);
val.setShowError(true);
val.setShowInput(true);
```

Similarly, if the requirement is remove the data validation rule from a single GridCell then its removeValidation method can be used to achieve the goal.

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Ability to create custom command buttons for Aspose.Cells.GridWeb for Java.
*   Ability to directly calculate the custom functions without inserting the function in worksheet.
*   Ability to export DataBar, ColorScale and IconSet of conditional formatting to HTML format.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][2].
*   [Aspose.Cells for Java Download Section][3].
*   [Aspose.Cells for Java Documentation][4] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][7] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][8] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/cells/java
[2]: https://products.aspose.com/cells/java
[3]: https://downloads.aspose.com/cells/java
[4]: https://docs.aspose.com/cells/java
[5]: https://apireference.aspose.com/cells/java
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://github.com/asposecells/Aspose_Cells_Java




