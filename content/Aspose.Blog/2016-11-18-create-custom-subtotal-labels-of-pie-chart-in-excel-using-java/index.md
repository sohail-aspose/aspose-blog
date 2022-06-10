---
title: 'Create Custom Subtotal Labels of Pie Chart in Excel using Java'
date: Fri, 18 Nov 2016 08:15:47 +0000
draft: false
url: /2016/11/18/create-custom-subtotal-labels-of-pie-chart-in-excel-using-java/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose team is pleased to announce the release of [Aspose.Cells for Java 16.11.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Create Custom Subtotal Labels in Excel using Java

Aspose.Cells for Java 16.11.0 has added the support for the creation of custom subtotal labels allowing the application developers to customize the labels according to the region or personal preferences. In order to provide this feature, the latest version of the Aspose.Cells for Java has exposed the GlobalizationSettings class offering the following 2 methods which can be overridden in a custom class to get desired labels for the Subtotals.

*   GlobalizationSettings.getTotalName: Gets the total name of the function.
*   GlobalizationSettings.getGrandTotalName: Gets the grand total name of the function.

The GlobalizationSettings class can be used to customize the Subtotal labels by overriding the GlobalizationSettings.getTotalName & GlobalizationSettings.getGrandTotalName methods as demonstrated ahead.

```
public class CustomSettings extends GlobalizationSettings
{    
    public String getTotalName(int functionType)
    {
    	 switch (functionType)
         {
             case ConsolidationFunction.AVERAGE:
                 return "AVG";

             //Handle other cases

             default:
                return super.getTotalName(functionType);
         }
    }

    public String getGrandTotalName(int functionType)
    {
    	 switch (functionType)
         {
             case ConsolidationFunction.AVERAGE:
                 return "GRAND AVG";

             //Handle other cases

             default:
            	 return super.getGrandTotalName(functionType);
         }      
    }
} 
```

In order to inject custom labels, it is required to assign the WorkbookSettings.GlobalizationSettings property to an instance of the CustomSettings class defined above, before adding the Subtotals to the worksheet

```
//Loads an existing spreadsheet containing some data
Workbook book = new Workbook(dir + "sample.xlsx");

//Assigns the GlobalizationSettings property of the WorkbookSettings class
//to the class created in first step
book.getSettings().setGlobalizationSettings(new CustomSettings());

//Accesses the 1st worksheet from the collection which contains data
//Data resides in the cell range A2:B9
Worksheet sheet = book.getWorksheets().get(0);

//Adds SubTotal of type Average to the worksheet
sheet.getCells().subtotal(CellArea.createCellArea("A2", "B9"), 0, ConsolidationFunction.AVERAGE, new int[] { 1 });

//Calculates Formulas
book.calculateFormula();

//Auto fits all columns
sheet.autoFitColumns();

//Saves the workbook on disc
book.save(dir + "output.xlsx");
```

## Render Custom Other Label for Pie Chart

The GlobalizationSettings class offers the getOtherName method which is useful to give the "Other" label of Pie charts a custom value. The following snippet defines a custom class and overrides the getOtherName method to get a custom label based on default language set for JVM.

```
public class CustomSettings extends GlobalizationSettings
{ 
    public String getOtherName()
    {
        String language = Locale.getDefault().getLanguage();
	System.out.println(language);
	switch (language)
	{
	    case "en":
	        return "Other";
	    case "fr":
	        return "Autre";
	    case "de":
	        return "Andere";

	    //Handle other cases as per requirement

	    default:
	        return super.getOtherName();
	}
    }
}
```

The following snippet loads an existing spreadsheet containing a Pie chart, and renders the chart to image while utilizing the CustomSettings class created above.

```
//Loads an existing spreadsheet containing a pie chart
Workbook book = new Workbook(dir + "sample.xlsx");

//Assigns the GlobalizationSettings property of the WorkbookSettings class
//to the class created in first step
book.getSettings().setGlobalizationSettings(new CustomSettings());

//Accesses the 1st worksheet from the collection which contains pie chart
Worksheet sheet = book.getWorksheets().get(0);

//Accesses the 1st chart from the collection
Chart chart = sheet.getCharts().get(0);

//Refreshes the chart
chart.calculate();

//Renders the chart to image
chart.toImage(dir + "output.png", new ImageOrPrintOptions());
```

Please check detailed article on [Introduction to GlobalizationSettings Class][4] if you want to get more in-depth knowledge of aforementioned usage scenarios.

## Create Style Object with CellsFactory Class

Aspose.Cells 16.11.0 has exposed the CellsFactory class which currently has one method, that is; createStyle. The CellsFactory.createStyle method can be used to create an instance of Style class without adding it to the pool of workbook styles.

Here is a simple usage scenario of newly exposed APIs to create a simple Style object, whereas a detailed article can be viewed on [Creating Style Object with CellsFactory Class][5].

```
//Initializes the CellsFactory class
CellsFactory factory = new CellsFactory();

//Creates an instance of Style
Style style = factory.createStyle();
```

## Access Hyperlink from a GridWeb

Aspose.Cells.GridWeb for Java 16.11.0 has exposed getHyperlink method to the GridHyperlinkCollection class that allows to get the instance of GridHyperlink by either passing an instance GridCell or a pair of integers corresponding to the row column indices.

Here is a simple usage scenario of GridHyperlinkCollection.getHyperlink method, whereas a detailed article can be viewed on [Access GridHyperlink from a GridCell Object][6].

```
//Gets the active worksheet from the collection
GridWorksheet sheet = gridWeb1.getWorkSheets().get(gridWeb1.getActiveSheetIndex());

//Accesses the GridHyperlinkCollection
GridHyperlinkCollection links = sheet.getHyperlinks();

//Gets hyperlink from cell A1
GridHyperlink link = links.getHyperlink(sheet.getCells().get("A1"));

//Gets hyperlink from cell D1
link = links.getHyperlink(0, 3);
```

## Other Enhancements & Fixes

Aspose.Cells for Java 16.11.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Support for [MINIFS & MAXIFS functions][7].
*   Ability to [manipulate Workbook's Absolute Path][8].
*   Enhanced Chart2Image module for accuracy of object positioning.

## Changes to the Public API

This revision of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow whereas details can be viewed from the [Migration Manual][9].

*   Constructor for the Style class has been marked obsoleted whereas an alternative approach has been exposed that uses the CellsFactory class.
*   The Cell.getConditionalStyle method has been completely removed from the public APIs because it was obsoleted some time back and an alternative approach has already been exposed by using Cell.getConditionalFormattingResult method.
*   The Cells.getMaxDataRowInColumn(int column) method has been removed. It is advised to use the Cells.getLastDataRow(int) method as an alternative.
*   The PageSetup.Draft property has been removed. It is advised to use the PageSetup.PrintDraft property instead.
*   The AutoFilter.FilterColumnCollection property has been removed while providing the AutoFilter.FilterColumns property to achieve the same goal.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][10].
*   [Aspose.Cells for Java Download Section][11].
*   [Aspose.Cells for Java Documentation][12] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][15] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cells/java/new-releases/aspose.cells-for-java-16.11.0/
[2]: https://docs.aspose.com/cells/java/release-notes/
[3]: https://docs.aspose.com/cells/java/upgrade-to-modern-aspose-cells-component/
[4]: https://docs.aspose.com/cells/java/using-globalizationsettings-class-for-custom-subtotal-labels-and-other-label-of-pie-chart/
[5]: https://docs.aspose.com/cells/java/create-style-object-using-cellsfactory-class/
[6]: https://docs.aspose.com/cells/java/access-hyperlink-object-of-the-gridweb-cell/
[7]: https://docs.aspose.com/cells/java/calculation-of-excel-2016-minifs-and-maxifs-functions/
[8]: https://docs.aspose.com/cells/java/change-the-absolute-path-of-external-link-data-source-file
[9]: https://docs.aspose.com/cells/java/public-api-changes-in-aspose-cells-16-11-0/
[10]: http://www.aspose.com/java/excel-component.aspx
[11]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[12]: https://docs.aspose.com/cells/java/
[13]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[16]: https://github.com/asposecells/Aspose_Cells_Java




