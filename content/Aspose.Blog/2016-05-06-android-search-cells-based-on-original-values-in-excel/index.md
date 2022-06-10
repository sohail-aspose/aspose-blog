---
title: 'Customize Calculation Engine and Search Cells Based on Original Values in Excel - Android API'
date: Fri, 06 May 2016 12:56:16 +0000
draft: false
url: /2016/05/06/android-search-cells-based-on-original-values-in-excel/
author: Babar Raza
summary: ''
tags: ['Android Excel APIs', 'Custom Calculation', 'Custom XML Parts', 'Excel Spreadsheets', 'ListObjects', 'Query Table', 'Search Cells', 'calculation engine', 'pivot table']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android 8.8.0][1]. This release includes a number of new features, enhancements and bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Implement Custom Calculation Engine

Aspose.Cells APIs have powerful calculation engine that can calculate almost all of the Microsoft Excel functions with precision. However, sometimes the application requirement demands to override any Excel formula in order to get desired results, such as return 3 for function **\=SUM(1,1)**, which isn't possible with default Aspose.Cells calculation engine.

The recent revision of Aspose.Cells for Android allows to extend the default calculation engine to get desired results. Aspose.Cells for Android 8.8.0 has exposed two new classes for this purpose as detailed below.

*   AbstractCalculationEngine: Represents custom calculation engine to extend the default calculation engine of Aspose.Cells.
*   CalculationData: Represents the required data when calculating one function, such as function name, parameters and so forth.

By implementing custom calculation engine, users can override all Excel's native functions with more flexibility. Below provided is the simplest usage scenario to define a custom calculation engine that extends AbstractCalculationEngine in order to override the Excel's default SUM function.

```
public class CustomEngine extends AbstractCalculationEngine
{
	public void calculate(CalculationData data)
        {
		if(data.getFunctionName().toUpperCase().equals("SUM")==true)
                {
                    double val = (double)data.getCalculatedValue();
                    val = val + 30;

                    data.setCalculatedValue(val);
                }
        }
}
```

Here is how to use the newly defined custom calculation engine to get desired results.

```
Workbook workbook = new Workbook();

Worksheet sheet = workbook.getWorksheets().get(0);

Cell a1 = sheet.getCells().get("A1");
a1.setFormula("=Sum(B1:B2)");

sheet.getCells().get("B1").putValue(10);
sheet.getCells().get("B2").putValue(10);

//Without overriding the SUM function, the value of cell A1 will be 20
workbook.calculateFormula();

System.out.println("Without Custom Engine Value of A1: " + a1.getStringValue());

//After overriding the SUM function, the value of cell A1 will be 50
CustomEngine engine = new CustomEngine();

CalculationOptions opts = new CalculationOptions();
opts.setCustomEngine(engine);

workbook.calculateFormula(opts);

System.out.println("With Custom Engine Value of A1: " + a1.getStringValue());
```

## Search in Cells Based on Original Values

Aspose.Cells APIs already support the Find or Search Data feature for spreadsheets in order to find some particular piece of contents in cell value & formula. However, this feature was lacking the aspect of formatting applied onto the cell that may change the appearance as well as the value of the cell, consequently making the content unsearchable using the original value. With this release of Aspose.Cells for Android API, another constant by the name LookInType.ORIGINAL\_VALUES has been exposed to the public API which allows to overcome the situation as discussed above.

The following piece of code demonstrates the usage of LookInType.ORIGINAL\_VALUES property to search the cells based on original values.

```
//Create workbook object
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Add 10 to cells A1 and A2
worksheet.getCells().get("A1").putValue(10);
worksheet.getCells().get("A2").putValue(10);

//Add Sum formula to cell D4
Cell cell = worksheet.getCells().get("D4");
cell.setFormula("=Sum(A1:A2)");

//Format the value to show as --- instead of original value
Style style = cell.getStyle();
style.setCustom("---");
cell.setStyle(style);

//Calculate the workbook
workbook.calculateFormula();

//Create find options and search for value 20
FindOptions options = new FindOptions();
options.setLookInType(LookInType.ORIGINAL_VALUES);
options.setLookAtType(LookAtType.ENTIRE_CONTENT);

Cell foundCell = null;
Object obj = 20;

//Find 20 which is Sum(A1:A2) and formatted as ---
foundCell = worksheet.getCells().find(obj, foundCell, options); 
```

## Control the Conversion of Large Numeric Value to Exponential Notation

As per default behaviour, if a numeric value is larger than the threshold, the API converts such values to exponential notation while importing HTML segment/files to Aspose.Cells object model. In past, we could use the HTMLLoadOptions.ConvertNumericData property to control the conversion of textual values to numeric data, however, this approach has its own drawbacks. For instance, if there are more than one columns containing the numeric values, setting the HTMLLoadOptions.ConvertNumericData property to false will direct the Aspose.Cells APIs to keep all values in textual format. In such case, all formatting from the numeric values will be lost.

In order to handle the situations where users wish to retain the format of all numeric values as well as keep the data in its original state, the Aspose.Cells for Android 8.8.0 has exposed the HTMLLoadOptions.KeepPrecision property. The Boolean type property allows to control the conversion of large numeric values to exponential notation. When set to true, the numeric values larger than 15 digits will be imported as it is.

Here is the simple usage scenario demonstrating the usage of HTMLLoadOptions.KeepPrecision property to avoid the conversion of large numbers to exponential notation while importing data from Html.

```
//Sample Html containing large number with digits greater than 15
String html = "<html><body>1234567890123456</body></html>";
//Convert Html to byte array
byte[] byteArray = html.getBytes();

//Set Html load options and keep precision true
HTMLLoadOptions loadOptions = new HTMLLoadOptions(LoadFormat.HTML);
loadOptions.setKeepPrecision(true);

//Convert byte array into stream
java.io.ByteArrayInputStream stream = new java.io.ByteArrayInputStream(byteArray);

//Create workbook from stream with Html load options
Workbook workbook = new Workbook(stream, loadOptions); 
```

## Add Custom XML Parts to Spreadsheets

Custom XML parts are the XML based data files stored by different applications like SharePoint inside the spreadsheet files. This data is consumed by different applications, however, Microsoft Excel application does not make use of this data so there is no GUI to add such data in the spreadsheets. One can view this data by extracting the contents of the spreadsheet (XLSX) using applications such as WinRar, and inspect the contents of the customXml folder.

Aspose.Cells for Android API provides the ContentTypePropertyCollection.add which can be used to add Custom XML data to the spreadsheet as demonstrated below.

```
//Create an instance of Workbook
Workbook workbook = new Workbook();

//Add custom XML to the collection of ContentTypeProperty objects 
workbook.getContentTypeProperties().add("BookStore", booksXML);
```

## Access TextBox from Collection

Aspose.Cells for Android 8.8.0 has exposed the overloaded indexer for the TextBoxCollection class in order to access the instance of TextBox using its name as demonstrated below.

```
//Create an instance of Workbook
Workbook workbook = new Workbook();

//Access the first Worksheet from the collection
Worksheet sheet = workbook.getWorksheets().get(0);

//Add a TextBox to the collection
int idx = sheet.getTextBoxes().add(10, 10, 10, 10);

//Access the TextBox using its index
TextBox box = sheet.getTextBoxes().get(idx);

//Set the name for the TextBox
box.setName("MyTextBox");

//Access the same TextBox via its name
box = sheet.getTextBoxes().get("MyTextBox"); 
```

## Detect if Cell Value Starts with Single Quote

Aspose.Cells for Android 8.8.0 has exposed the Style.QuotePrefix property to detect if the cell value starts with single quote mark. With previous revisions of Aspose.Cells APIs, it was not possible to distinguish between the text values such as sample and 'sample.

Here is the simple usage scenario of Style.QuotePrefix property to find if the cell value starts with single quote mark.

```
//Create an instance of workbook
Workbook workbook = new Workbook();

//Access first worksheet from the collection
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access cells A1 and A2
Cell a1 = worksheet.getCells().get("A1");
Cell a2 = worksheet.getCells().get("A2");

//Add simple text to cell A1 and text with quote prefix to cell A2
a1.putValue("sample");
a2.putValue("'sample");

//Print their string values, A1 and A2 both are same
System.out.println("String value of A1: " + a1.getStringValue());
System.out.println("String value of A2: " + a2.getStringValue());

//Access styles of cells A1 and A2
Style s1 = a1.getStyle();
Style s2 = a2.getStyle();

System.out.println();

//Check if A1 and A2 has a quote prefix
System.out.println("A1 has a quote prefix: " + s1.getQuotePrefix());
System.out.println("A2 has a quote prefix: " + s2.getQuotePrefix()); 
```

## Delete Redundant Spaces from HTML

Aspose.Cells for Android has exposed the HTMLLoadOptions.DeleteRedundantSpaces property to control the preservation of redundant spaces after the line break tag (<BR> tag) in HTML. If the aforementioned property is set to true the API will delete all the redundant spaces while importing the HTML in Aspose.Cells object mode. The HTMLLoadOptions.DeleteRedundantSpaces property has the default value as false, that means, all the redundant spaces are preserved in the resultant spreadsheet.

## Access Query Table Properties

Aspose.Cells APIs have exposed the Boolean type QueryTable.PreserveFormatting & QueryTable.AdjustColumnWidth properties in order to mimic the Excel's features of preserving cell formatting & adjusting column widths while working with External Data Range of type Query Table.

Please note, Excel application provides these options to influence the formatting of the data where the options can be accessed on Excel interface from **Data** tab by clicking the **Properties** button as shown below.

The following piece of code shows the simple usage scenario of QueryTable.PreserveFormatting &QueryTable.AdjustColumnWidth properties.

```
//Create an instance of Workbook from existing spreadsheet
Workbook workbook = new Workbook(inFilePath);

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access first Query Table from the collection
QueryTable qt = worksheet.getQueryTables().get(0);

//Print Query Table properties
System.out.println("Adjust Column Width: " + qt.getAdjustColumnWidth());
System.out.println("Preserve Formatting: " + qt.getPreserveFormatting());

//Set Preserve Formatting to true
qt.setPreserveFormatting(true);

//Save the workbook
workbook.save(outFilePath); 
```

## Enhancements to Formula Calculation Engine

Aspose.Cells APIs have enhanced the formula calculation engine with this release where the most worth mentioning enhancements are as follow.

### Support for Array Formulas of Data Tables

In perspective of Excel application, Data tables are part of a suite of commands that are called what-if analysis tools. These tools can be used to process the formulas by changing the values in cells to see how those changes will affect the outcome of formulas on the worksheet. With this release of Aspose.Cells for Android, the API now allows you to calculate the array formula of Data Tables. Please note, no new API have been exposed for this feature and all enhancements are done internally to the formula calculation engine therefore by simply calling the Workbook.calculateFormula method, all formulas including the array formulas will be computed automatically.

### Support for FORMULATEXT Function

Aspose.Cells for Android has provided support for the Excel's FORMULATEXT Function which can be used to get the formula string for any given cell as it is being displayed in the Excel's formula bar.

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Ability to use image markers while grouping data in smart markers.
*   Ability to find Query Tables and List Objects related to external data connections.




[1]: http://www.aspose.com/downloads/cells-family/android/new-releases/aspose.cells-for-android-8.8.0/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java




