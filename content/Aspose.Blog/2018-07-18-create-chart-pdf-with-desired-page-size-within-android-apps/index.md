---
title: 'Create Chart PDF with Desired Page Size within Android Apps'
date: Wed, 18 Jul 2018 10:40:11 +0000
draft: false
url: /2018/07/18/create-chart-pdf-with-desired-page-size-within-android-apps/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 18.6][1]. This release includes many new features, enhancements and other bug fixes that further improve the overall stability and usability of the API. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a look at the most worth mentioning features in this release

## Create Chart PDF with Desired Page Size

You can create chart's PDF file with your desired page size using Aspose.Cells and specify how you want to align the chart inside the page as top, bottom, center, left, right etc. Besides this, the output chart can be created in stream or on disk. Please see the following article for more detail on this topic.

*   [Create Chart PDF with Desired Page Size][4]

## Rotate Text with Shape inside the Worksheet

You can add text inside any shape using Microsoft Excel. If you add shape using the older Microsoft Excel 2003, then text will not rotate with shape. But if you add shape using newer versions of Microsoft Excel e.g. 2007, 2010, 2013 or 2016 etc. then text will be rotated with shape. You can control if the text should rotate with shape or not using the **ShapeTextAlignment.RotateTextWithShape** property.

*   [Rotate Text with Shape inside the Worksheet][5]

## Read/Write TSV (Tab-Separated Values) Files

TSV files are used to contain spreadsheet data but without any formatting. The format is same with Tab Delimited where data is arranged in rows and columns such as tables and spreadsheets. To open tab delimited files, developers should call the **LoadOptions** method and select the **TSV** value, predefined in the **FileFormatType** enumeration. Please see the following sample code and the related article for your reference.

```
// Creating TSV LoadOptions object.
LoadOptions loadOptions = new LoadOptions(FileFormatType.TSV);

// Creating an Workbook object with TSV text file path and the LoadOptions object.
Workbook workbook = new Workbook(dirPath + "SampleTSVfile.tsv", loadOptions);

// Print success message.
System.out.println("TSV workbook has been opened successfully.");
```

*   [Opening Tab-Separated Values (TSV) Files][6]Files)

## Get All Hidden Rows Indices after Refreshing AutoFilter

When you apply auto filter on worksheet cells, then some of the rows get hidden automatically. But it might be the case that some of the rows are already hidden manually by MS Excel end user and they are not hidden by auto filter feature. It therefore makes difficult to know which of the rows are hidden by auto filter and which rows are hidden manually by MS Excel end user. Aspose.Cells deals with this problem using the **int\[\] AutoFilter.refresh(boolean hideRows)** method. This method returns the row indices of all the rows that are hidden by auto filter and not by manual way in MS Excel.

*   [Get All Hidden Rows Indices after Refreshing AutoFilter][7]

## Avoid Blank Page in Output Pdf when there is Nothing to Print

When the Excel file is empty and user saves it to PDF using Aspose.Cells, it renders blank page in output PDF. Sometime, this default behavior is undesirable. Aspose.Cells provides the **PdfSaveOptions.OutputBlankPageWhenNothingToPrint** property to deal with this issue. If you will set it as false, then CellsException will occur whenever there is nothing to print in the output PDF.

*   [Avoid Blank Page in Output Pdf when there is Nothing to Print][8]

## Find Type of X and Y Values of Points in Chart Series

Sometime, you want to know the type of X and Y values of chart points in a series. Aspose.Cells provides **ChartPoint.XValueType** and **ChartPoint.YValueType** properties that can be used for this purpose. Please note, you will have to call **Chart.calculate()** method before you could use these properties effectively.

*   [Find Type of X and Y Values of Points in Chart Series][9]

## Get HTML5 string from Cell

Aspose.Cells returns the HTML string of the cell using the string **Cell.getHtmlString (boolean html5)** method. If you pass "false" as parameter, it will return you Normal HTML but if you pass "true" as parameter, it will return Html5 string.

*   [Get HTML5 string from Cell][10]

## Hiding Overlaid Content with CrossHideRight while saving to Html

When you save your MS Excel file to HTML, you can specify different cross types for cell strings. By default, Aspose.Cells generates HTML as per Microsoft Excel but when you change cross type to **CrossHideRight** then it hides all the strings from the right side of the cell which are overlaid or overlapping with cell string.

*   Hiding Overlaid Content with CrossHideRight while saving to Html

## Specify the Language of the Excel File using Built In Document Properties

You can change the Language of MS Excel file by right clicking the file and then selecting Properties > Details and then editing the Language field. Please use **BuiltInDocumentPropertyCollection.Language** property to change it programmatically using Aspose.Cells APIs.

*   [Specify the Language of the Excel File using BuiltIn Document Properties][11]

## Specify the Far East and Latin Name of the Font in Text Options of Shape

Sometimes you want to display text in Far East language font e.g. Japanese, Chinese, Thai etc. Aspose.Cells provides **TextOptions.FarEastName** property that can be used to specify the font name of Far East language. Besides, you can also specify the Latin font name using **TextOptions.LatinName** property. Please see the following article for more detail on this topic.

*   [Specify the Far East and Latin Name of the Font in Text Options of Shape][12]

## Save Workbook to Strict Open XML Spreadsheet Format

Aspose.Cells allows you to save the workbook in Strict Open XML Spreadsheet format. For that purpose, it provides the **Workbook.Settings.Compliance** property. If you set its value as **OoxmlCompliance.ISO\_29500\_2008\_STRICT**, then the output Excel file will be saved in Strict Open XML Spreadsheet format.

```
// Create workbook.
Workbook wb = new Workbook();

// Specify - Strict Open XML Spreadsheet - Format.
wb.getSettings().setCompliance(OoxmlCompliance.ISO_29500_2008_STRICT);

// Add message in cell B4 of first worksheet.
Cell b4 = wb.getWorksheets().get(0).getCells().get("B4");
b4.putValue("This Excel file has Strict Open XML Spreadsheet format.");

// Save to output Excel file.
wb.save(dirPath + "outputSaveWorkbookToStrictOpenXMLSpreadsheetFormat.xlsx", SaveFormat.XLSX);
```

*   [Save Workbook to Strict Open XML Spreadsheet Format][13]

## Specify Individual or Private Set of Fonts for Workbook Rendering

Generally, you specify the fonts directory or list of fonts for all the workbooks but sometime, you have to specify individual or private set of fonts for your desired workbooks. Aspose.Cells provides **IndividualFontConfigs** class that can be used to specify the individual or private set of fonts for your workbook. Please see the following article for more detail on this topic.

*   [Specify Individual or Private Set of Fonts for Workbook Rendering  
    ](https://docs.aspose.com/cells/java/specify-individual-or-private-set-of-fonts-for-workbook-rendering/)

## Add Cells to Microsoft Excel Formula Watch Window

Microsoft Excel Watch Window is a useful tool to watch the cell values and its formulas conveniently in a window. You can open the Watch Window using Microsoft Excel by clicking the **Formulas > Watch Window**. It has **Add Watch** button that can be used to add the cells for inspection. Similarly, you can use **Worksheet.getCellWatches().add()** method to add cells into Watch Window using Aspose.Cells API. Please see the following article for more detail on this topic.

*   [Add Cells to Microsoft Excel Formula Watch Window][14]

## Working with Slicers using Aspose.Cells API

Slicers are used to filter data quickly. It provides buttons that user can click to filter Table or Pivot Table data. Whenever, Slicer buttons are selected or deselected, it shows the current filtering state that helps the user to understand what precisely has been filtered in the Pivot Table. Please see the following articles that explain how to work with Slicers using Aspose API.

*   [Create Slicer to a Pivot Table][15]
*   [Formatting Slicer][16]
*   [Removing Slicer][17]
*   [Rendering Slicer][18]
*   [Updating Slicer][19]

The following sample code loads an Excel file that contains an existing Slicer. It unselects the 2nd and 3rd items of Slicer to refresh it. It then applies formatting/style of the Slicer and finally describes on how to remove the Slicer.

```
// Load sample Excel file containing slicer.
Workbook wb = new Workbook(dirPath + "sampleUpdatingSlicer.xlsx");
 
// Access first worksheet.
Worksheet ws = wb.getWorksheets().get(0);
 
// Access the first slicer inside the slicer collection.
Slicer slicer = ws.getSlicers().get(0);
 
// Access the slicer items.
SlicerCacheItemCollection scItems = slicer.getSlicerCache().getSlicerCacheItems();
 
// Unselect 2nd and 3rd slicer items.
scItems.get(1).setSelected(false);
scItems.get(2).setSelected(false);
 
// Refresh the slicer.
slicer.refresh();

// Set the slicer style/formatting.
slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_6);

// Remove slicer.
ws.getSlicers().remove(slicer); 
```

## Add Custom XML Parts and Select them by ID

Custom XML Parts are the XML data that is stored inside the Microsoft Excel documents and are used by the applications that deal with them. There is no direct way of adding them using Microsoft Excel UI at the moment. However, you can add them programmatically in various ways e.g. using VSTO, using Aspose.Cells etc. Please use **Workbook.getCustomXmlParts().add()** method if you want to add Custom XML Part using Aspose.Cells API. You can also set its ID, using the **CustomXmlPart.ID** property. Similarly, if you want to select Custom XML Part by ID, you can use **Workbook.getCustomXmlParts().selectByID()** method.

*   [Add Custom XML Parts and Select them by ID][20]

## Get Address, CellCount Offset, EntireColumn and EntireRow of the Range

Aspose.Cells has added few new utility methods inside the Range object that help the user finding Address, Cell Count, Offset, Entire Column and Entire Row of the Range object. Please see the following article for more detail on this.

*   [Get Address, Cell Count, Offset, Entire Column and Entire Row of the Range][21]

## Extract Text from the Gear Type SmartArt Shape

Aspose.Cells can extract text from the Gear Type Smart Art Shape. In order to do so, you should first convert Smart Art Shape to Group Shape using the **Shape.getResultOfSmartArt()** method. Then you should get the array of all the Individual Shapes forming the Group Shape using the **GroupShape.getGroupedShapes()** method. Finally, you can iterate all of Individual Shapes one by one in a loop and extract their text using the **Shape.getText()** method.

*   [Extract Text from the Gear Type SmartArt Shape][22]

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][23].
*   [Aspose.Cells for Android via Java Download Section][24].
*   [Aspose.Cells for Android via Java Documentation][25] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][26] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][27] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][28] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][29] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.6/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/cells/java/aspose-cells-for-android-via-java-18-6-release-notes/
[4]: https://docs.aspose.com/cells/java/create-chart-pdf-with-desired-page-size/
[5]: https://docs.aspose.com/cells/java/rotate-text-with-shape-inside-the-worksheet/
[6]: https://docs.aspose.com/cells/java/opening-files-with-different-formats/#OpeningFileswithDifferentFormats-OpeningTab-SeparatedValues(TSV
[7]: https://docs.aspose.com/cells/java/get-all-hidden-rows-indices-after-refreshing-autofilter/
[8]: https://docs.aspose.com/cells/java/avoid-blank-page-in-output-pdf-when-there-is-nothing-to-print/
[9]: https://docs.aspose.com/cells/java/find-type-of-x-and-y-values-of-points-in-chart-series/
[10]: https://docs.aspose.com/cells/java/get-html5-string-from-cell/
[11]: https://docs.aspose.com/cells/java/specify-the-language-of-the-excel-file-using-builtin-document-properties/
[12]: https://docs.aspose.com/cells/java/specify-the-far-east-and-latin-name-of-the-font-in-text-options-of-shape/
[13]: https://docs.aspose.com/cells/java/save-workbook-to-strict-open-xml-spreadsheet-format/
[14]: https://docs.aspose.com/cells/java/add-cells-to-microsoft-excel-formula-watch-window/
[15]: https://docs.aspose.com/cells/java/create-slicer-to-a-pivot-table/
[16]: https://docs.aspose.com/cells/java/formatting-slicer/
[17]: https://docs.aspose.com/cells/java/removing-slicer/
[18]: https://docs.aspose.com/cells/java/rendering-slicer/
[19]: https://docs.aspose.com/cells/java/updating-slicer/
[20]: https://docs.aspose.com/cells/java/add-custom-xml-parts-and-select-them-by-id/
[21]: https://docs.aspose.com/cells/java/get-address-cell-count-offset-entire-column-and-entire-row-of-the-range/
[22]: https://docs.aspose.com/cells/java/extract-text-from-the-gear-type-smartart-shape/
[23]: https://products.aspose.com/cells/java/
[24]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.6/
[25]: https://docs.aspose.com/cells/java/
[26]: https://apireference.aspose.com/java/cells
[27]: https://forum.aspose.com/c/cells
[28]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[29]: https://github.com/asposecells/Aspose_Cells_Java




