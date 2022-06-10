---
title: 'Optimize PDF, Re-size Data Label to Fit Text with Aspose.Cells for Android 8.7.0'
date: Fri, 12 Feb 2016 08:38:01 +0000
draft: false
url: /2016/02/12/optimize-pdf-re-size-data-label-to-fit-text-in-excel-spreadsheets/
author: Babar Raza
summary: ''
tags: ['2-Color Scale', 'Aspose.Cells for Android', 'Babar Raza', 'CSV', 'Excel API', 'Excel API for Android', 'Excel File Manipulation', 'Excel Formulas', 'Excel Function', 'Excel to HTML', 'Optimize PDF', 'Render Chart to PDF', 'Resize shape to fit text', 'Worksheet Password', 'Worksheet Protection', 'conditional formatting', 'spreadsheet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


Aspose.Cells for Android 8.7.0 is now available for public use. This release contains many useful features and improvements along with some important bug fixes. Have a look at the release notes of [Aspose.Cells for Android 8.7.0][1] for complete details. While you are downloading the latest release, here is a quick overview of some of the most worth mentioning features.

## Optimize PDF File Size

Aspose.Cells APIs have provided an enhancement to the PDF rendering engine in order to reduce the resultant PDF file size. Aspose.Cells for Android 8.7.0 has exposed the PdfSaveOptions.OptimizationType property along with an enumeration PdfOptimizationType in order to facilitate the application developers to control the resultant PDF file size to some extent.

The PdfOptimizationType enumeration has 2 constants at the moment exhibiting the following behaviour.

1.  PdfOptimizationType.MINIMUM\_SIZE: API tries to optimize the cell text and cell border records in order to reduce the resultant PDF file size.
2.  PdfOptimizationType.STANDARD: No optimization is done therefore the resultant file size will be large as compared to PdfOptimizationType.MINIMUM\_SIZE selection.

## Re-size Chart's Data Label Shape to Fit Text

Aspose.Cells for Android 8.7.0 has exposed the Boolean type DataLabels.ResizeShapeToFitText property in order to mimic the Excel's feature of re-sizing data label shapes to fit the text.

Please note, Excel application provides the **Resize shape to fit text** option for chart's data labels to increase the size of the shape so that the text fits inside of it. This option can be accessed on Excel interface by selecting any of the data labels on the chart. Right click and select **Format DataLabels** menu. On **Size & Properties** tab, expand **Alignment** node to reveal the related properties including the **Resize shape to fix text** option as highlighted below.



{{< figure align=center src="images/Excel-Resize-Shape-To-Fit-Text.png" alt="">}}


The following piece of code shows the simple usage scenario of DataLabels.ResizeShapeToFitText property to re-size the chart's data label shapes to fit text.

```
//Create an instance of Workbook containing the Chart
Workbook book = new Workbook(inFilePath);

//Access the Worksheet that contains the Chart
Worksheet sheet = book.getWorksheets().get(0);

//Access ChartCollection from Worksheet
ChartCollection charts = sheet.getCharts();

//Loop over each chart in collection
for (int chartIndex = 0; chartIndex < charts.getCount(); chartIndex++)
{
	//Access indexed chart from the collection
	Chart chart = charts.get(chartIndex);

	for (int seriesIndex = 0; seriesIndex < chart.getNSeries().getCount(); seriesIndex++)
	{
	    //Access the DataLabels of indexed NSeries
		DataLabels labels = chart.getNSeries().get(seriesIndex).getDataLabels();

	    //Set ResizeShapeToFitText property to true
	    labels.setResizeShapeToFitText(true);
	}

	//Calculate Chart
	chart.calculate();
}

//Save the result
book.save(outFilePath); 
```

Here is a snapshot showing a simple bar chart before & after executing the above code.



{{< figure align=center src="images/chart-resize-datalabel-shape-to-fit-text.png" alt="">}}


## Enhancements to Protection Module

Aspose.Cells APIs have enhanced the Protection class by introducing some useful properties & methods. Two of the most worth mentioning enhancements are as follow.

### Detect if Worksheet is Password Protected

It is possible to protect the workbooks and worksheets separately. For instance, a spreadsheet may contain one or more worksheets that are password protected, however, the spreadsheet itself may or may not be protected. Aspose.Cells API for Java has provided the Protection.isProtectedWithPassword field to detect if a worksheet is password protected. Boolean type Protection.isProtectedWithPassword field returns true if Worksheet is password protected and false if not.

### Verify Password Used to Protect the Worksheet

Aspose.Cells for Android 8.7.0 has exposed the Protection.verifyPassword method which allows to specify a password as an instance of String and verifies if same password has been used to protect the worksheet. The Protection.verifyPassword method returns true if the specified password matches with the password used to protect the given Worksheet, false if specified password does not match.

## Load or Import Delimited File Containing Formulas

Aspose.Cells for Android has provided support to identify & parse the formulas while loading CSV/TXT files having delimited plain data. Newly exposed TxtLoadOptions.HasFormula property when set to true directs the API to parse the formulas from the input delimited file and set them to relevant cells without requiring any additional processing.

The following piece of code demonstrates the usage of TxtLoadOptions.HasFormula property to load and import the CSV with formulas in it.

```
TxtLoadOptions opts = new TxtLoadOptions();
opts.setSeparator(',');
opts.setHasFormula(true);

//Load your CSV file with formulas in a Workbook object
Workbook workbook = new Workbook(csvFile, opts);

//You can also import your CSV file by importing it onto the Worksheet cells
//The code below is importing CSV file starting from cell D4
Worksheet worksheet = workbook.getWorksheets().get(0);
worksheet.getCells().importCSV(csvFile, opts, 3, 3); 
```

## Set Link Target Type for HTML Conversion

Aspose.Cells APIs are capable of converting all supported spreadsheet formats to HTML with highest fidelity. The conversion process is efficient as well as configurable to meet any application requirements. Aspose.Cells for Android APIs have exposed the HtmlSaveOptions class that is mainly responsible for the conversion process and provides a vast array of features to influence the HTML generation process.

This release of Aspose.Cells for Android has exposed an enumeration namely HtmlLinkTargetType along with a new property HtmlSaveOptions.LinkTargetType that together allows to set the target type for the links in spreadsheet while conversion to HTML format. The possible values of the HtmlLinkTargetType enumeration are as follow where the default value is SELF.

*   HtmlLinkTargetType.BLANK: Opens the linked document/page in a new window or tab.
*   HtmlLinkTargetType.PARENT: Opens the linked document/page in parent frame.
*   HtmlLinkTargetType.SELF: Opens the linked document/page in the same frame where the link was clinked.
*   HtmlLinkTargetType.TOP: Opens the linked document/page in the full body of the window.

## Directly Render Chart to PDF

The Aspose.Cells for Android has introduced the Chart.toPdf method in order to simplify the task of rendering charts in PDF format. Previous solution was to copy the required chart onto a new Worksheet then render the worksheet to PDF while specifying the area containing the chart shape. This solution was prone to error due to the number of statements to accomplish the same goal that can now be achieved in a single statement. The Chart.toPdf method currently accepts a parameter of type String as file path location to store the resultant PDF directly onto the disk.

## Access & Update Portion of Rich Text

Aspose.Cells for Android now provides an easy to use mechanism to access the format related properties of each character from a cell containing Rich Text. The API has exposed the getCharacters & setCharacters methods for the Cell class that allows to access & update the portion of the Rich Text in a cell. The Cell.getCharacters method returns an array of FontSetting objects where each object represents the styling of an individual character. The Cell.setCharacters method also accepts an array of FontSetting objects to set the styling for individual characters of a cell.

## Load Only Visible Worksheets from Existing Spreadsheet

Aspose.Cells APIs provide a set of classes for the developers to influence the spreadsheet loading mechanism. While using the LoadOptions & LoadDataOptions classes, the developers can set a number of options such as force the API to load specific worksheets, where the worksheets can be specified via their indices or names.

Aspose.Cells for Android has exposed another useful property for the LoadDataOptions class which allows to load only the visible worksheets from an existing spreadsheet, where the hidden worksheets will be simply ignored and will not be available in the Aspose.Cells object model for any processing. The newly exposed property LoadDataOptions.OnlyVisibleWorksheet is of type Boolean; setting it to true means that the API will ignore the hidden worksheets and load only the visible worksheets for further processing.

## Remove Unused Styles from Workbook's Style Pool

It is fairly possible that a spreadsheet may contain styles that are not in use. Such scenario may easily occur when user copies cells from another workbook because in this case some styles are copied too. Due to the reason that styles are shared for many objects such as cells, rows, columns and so on, when one cell's content (including style) is replaced by the copied one, the Aspose.Cells APIs do not remove the old style from the style pool. Imagine if the user does the copy operation repeatedly, there will be more and more styles in the style pool. Such unused styles can now be removed from the object of the Workbook while using the newly exposed removeUnusedStyles method. However, the aforementioned method could impose performance plenty because it has to check all objects to make sure that one style is not being used by any object, so we recommend to use this method with great caution.

## Create Excel's Built-in Styles

Aspose.Cells for Android has exposed the Workbook.createBuiltinStyle method that can be used to create an object of the Style class that corresponds to one of the built-in styles offered by the Excel application. The Workbook.createBuiltinStyle method accepts a constant from the enumeration BuiltinStyleType.

Please note, with previous releases of the Aspose.Cells APIs, same task could be accomplished via StyleCollection.createBuiltinStyle method but as the recent releases of Aspose.Cells APIs have removed the StyleCollection class from the public API therefore the newly exposed Workbook.createBuiltinStyle method can be considered as an alternative approach to achieve the same goal.

## Create 2-Color Scale Conditional Format

This release of the API has has exposed the ColorScale.Is3ColorScale property that can be used to create 2-Color Scale conditional format. The said property is of type boolean with default value of true which means that the conditional format will be of 3-Color Scale by default. However, switching the ColorScale.Is3ColorScale property to false will generate a 2-Color Scale conditional format.

Following is the simple usage scenario to generate 2-color scale conditional format. Please also review the detailed article on Adding 2 & 3-Color Scale Conditional Formatting.

```
//Create an instance of Workbook
//Optionally load an existing spreadsheet
Workbook book = new Workbook();

//Access the Worksheet to which conditional formatting rule has to be added
Worksheet sheet = book.getWorksheets().get(0);

//Add FormatConditions to the collection
int index = sheet.getConditionalFormattings().add();

//Access newly added formatConditionCollection via its index
FormatConditionCollection formatConditionCollection = sheet.getConditionalFormattings().get(index);

//Create a CellArea on which conditional formatting rule will be applied
CellArea cellArea = CellArea.createCellArea("A1", "A5");

//Add conditional formatted cell range
formatConditionCollection.addArea(cellArea);

//Add format condition of type ColorScale
index = formatConditionCollection.addCondition(FormatConditionType.COLOR_SCALE);

//Access newly added format condition via its index
FormatCondition formatCondition = formatConditionCollection.get(index);

//Set Is3ColorScale to false in order to generate a 2-Color Scale format
formatCondition.getColorScale().setIs3ColorScale(false);

/*
Set other necessary properties
*/ 
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Newly exposed field VbaProject.isSigned allows to detect if a given VbaProject is digitally signed or not.
*   This release has added support for importing XML map inside an instance of Workbook.
*   Another worth mentioning feature of this release is the ability to work with external data connection of type Web Query.

## Aspose.Cells for Android Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android API][2].
*   [Aspose.Cells for Android Download Section][3].
*   [Aspose.Cells for Android Documentation][4] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   Aspose.Cells for Android API Reference Guide – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Cells for Android Examples – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Aspose.Cells Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][6] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.




[1]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry686635.aspx
[2]: https://products.aspose.com/cells/android-java/
[3]: https://downloads.aspose.com/cells/android-java/
[4]: https://docs.aspose.com/cells/androidjava/
[5]: https://forum.aspose.com/
[6]: https://blog.aspose.com/




