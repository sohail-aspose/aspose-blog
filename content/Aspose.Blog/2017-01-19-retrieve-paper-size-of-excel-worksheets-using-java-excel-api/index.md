---
title: 'Retrieve Paper Size of Excel Worksheets using Java'
date: Thu, 19 Jan 2017 11:47:25 +0000
draft: false
url: /2017/01/19/retrieve-paper-size-of-excel-worksheets-using-java-excel-api/
author: Babar Raza
summary: ''
tags: ['Custom Format', 'Excel Component', 'Excel Java API', 'Glow Effect', 'PageSetup', 'Rendering Excel in Java', 'Significant Digits', 'Verify Custom Pattern']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose team is pleased to announce the release of [Aspose.Cells for Java 17.1.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Get Paper Size of the Worksheet using Java

Sometimes, the application requirement could be to retrieve the worksheet's paper size in the unit of Inches, which can now be achieved using the PageSetup.PaperWidth and PageSetup.PaperHeight properties. The PageSetup.PaperWidth and PageSetup.PaperHeight properties are of type double representing the paper width & height in the unit of inches while considering the page orientation.

The following code snippet tries to explain the usage of PageSetup.PaperWidth and PageSetup.PaperHeight properties. Please review the detailed article if you wish to get more in-depth knowledge on how to get the worksheet's paper size.

```
//Create workbook
Workbook book = new Workbook();

//Access first worksheet
Worksheet sheet = book.getWorksheets().get(0);

//Set paper size to A2 and print paper width and height in inches
sheet.getPageSetup().setPaperSize(PaperSizeType.PAPER_A_2);
System.out.println("PaperA2: " + sheet.getPageSetup().getPaperWidth() + "x" + sheet.getPageSetup().getPaperHeight());

//Set paper size to A3 and print paper width and height in inches
sheet.getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
System.out.println("PaperA3: " + sheet.getPageSetup().getPaperWidth() + "x" + sheet.getPageSetup().getPaperHeight());

//Set paper size to A4 and print paper width and height in inches
sheet.getPageSetup().setPaperSize(PaperSizeType.PAPER_A_4);
System.out.println("PaperA4: " + sheet.getPageSetup().getPaperWidth() + "x" + sheet.getPageSetup().getPaperHeight());

//Set paper size to Letter and print paper width and height in inches
sheet.getPageSetup().setPaperSize(PaperSizeType.PAPER_LETTER);
System.out.println("PaperLetter: " + sheet.getPageSetup().getPaperWidth() + "x" + sheet.getPageSetup().getPaperHeight()); 
```

## Improved Custom Load Filtering Mechanism

The LoadFilter class allows to customize the loading process as per the properties of the Worksheet. In order to customize the loading process, one has to override the LoadFilter.startSheet method. Please note, there are just a few properties that can be used for a given worksheet object in this scenario because most of the data and properties have not been loaded yet. The available Worksheet properties are: Name, Index & VisibilityType.

With the release of Aspose.Cells for Java 17.1.0, the API has added the setter for the LoadFilter.LoadDataFilterOptions property to replace the m\_LoadDataFilterOptions instance variable. Users may change the LoadDataFilterOptions property in their own implementation of LoadFilter class to control the behavior of loading template files.

Following snippet demonstrates how to extend the LoadFilter class and override the startSheet method in order to choose different loading mechanism as per worksheets in a given template.

```
class CustomLoadFilter extends LoadFilter {
	public void startSheet(Worksheet sheet) {

		if (sheet.getName().equals("NoCharts")) {
			//Load everything and filter charts
			this.setLoadDataFilterOptions(LoadDataFilterOptions.ALL& ~LoadDataFilterOptions.CHART);
		}

		if (sheet.getName().equals("NoShapes")) {
			//Load everything and filter shapes
			this.setLoadDataFilterOptions(LoadDataFilterOptions.ALL& ~LoadDataFilterOptions.SHAPE);
		}

		if (sheet.getName().equals("NoConditionalFormatting")) {
			//Load everything and filter conditional formatting
			this.setLoadDataFilterOptions(LoadDataFilterOptions.ALL& ~LoadDataFilterOptions.CONDITIONAL_FORMATTING);
		}
	}
} 
```

The newly created class can be used as follow.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Set the LoadFilter property of LoadOptions object to the instance of CustomFilter class created above
options.setLoadFilter(new CustomFilter());

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

In order to get a more in-depth understanding of the new filtering mechanism, please check the detailed article on [Filtering Objects at Load Time][4].

## Specify the Number of Significant Digits

Aspose.Cells APIs store 17 significant digits of double values unlike Excel application which stores only 15 significant digits. You can override this default behavior of Aspose.Cells APIs while using the newly exposed CellsHelper.SignificantDigits property.

The following code snippet enforces the Aspose.Cells APIs to use 15 significant digits while storing double values to the spreadsheet files of type XLSX. Please review the detailed article if you wish to get more in-depth knowledge on [how to specify significant digits][5].

```
//Specify the number of significant digits
CellsHelper.setSignificantDigits(15);

//Create workbook
Workbook book = new Workbook();

//Access first worksheet
Worksheet sheet = book.getWorksheets().get(0);

//Access cell A1
Cell cell = sheet.getCells().get("A1");

//Put double value, only 15 significant digits as specified by
//CellsHelper.SignificantDigits above will be stored in spreadsheet
cell.putValue(1234567890.123451711);

//Save the workbook
book.save(dir + "output.xlsx"); 
```

## Verify Custom Pattern for the Style Object

Aspose.Cells for Java 17.1.0 has added the CheckCustomNumberFormat property to the WorkbookSettings class. The CheckCustomNumberFormat is useful in [checking if the Style.Custom property has been set properly][6] or not. In case the Style.Custom property has been set improperly, that is; the value does not correspond to valid pattern then the Aspose.Cells for Java APIs will throw CellsException with appropriate message.

The following code snippet tried to assign an invalid custom format to the Style.Custom property. Since, the code has already set WorkbookSettings.CheckCustomNumberFormat property to true therefore the statement to set the Style.Custom property will cause CellsException.

```
//Create an instance of Workbook
Workbook book = new Workbook();

//Set CheckCustomNumberFormat property to true
book.getSettings().setCheckCustomNumberFormat(true);

//Access first worksheet
Worksheet sheet = book.getWorksheets().get(0);

//Access a cell
Cell cell = sheet.getCells().get("B5");

//Insert a value to the cell
cell.putValue(2347);

//Access cell's style
Style style = cell.getStyle();
         
//Set Custom property to an invalid pattern
style.setCustom("ggg @ fff");

//Set the modified style to the cell
cell.setStyle(style); 
```

## Other Enhancements & Fixes

Aspose.Cells for Java 17.1.0 has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Ability to read the color of shape's glow effect.
*   Support for rendering gradient fill for WordArt objects while converting spreadsheets to HTML.
*   Support to load Excel 2016 chart types.
*   Enhanced HTML parsing engine for inline CSS.
*   Handled a few exceptions such as ArrayIndexOutOfBoundsException & NullPointerException.

## Changes to the Public API

This revision of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow whereas details can be viewed from the [Migration Manual][7].

*   Several new fields have been added to the ChartType enumeration which represents chart types specific to Excel 2016.
*   A new field Percentage has been added to the DisplayUnitType enumeration that indicates the values on the chart shall be divided by 0.01.
*   The instance variable m\_LoadDataFilterOptions has been removed. It is advised to use the LoadFilter.LoadDataFilterOptions property instead.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][8].
*   [Aspose.Cells for Java Download Section][9].
*   [Aspose.Cells for Java Documentation][10] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.1.0/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.1.0+Release+Notes
[3]: https://docs.aspose.com/cells/java/migrating-from-earlier-versions-of-aspose-cells/
[4]: https://docs.aspose.com/cells/java/filter-objects-while-loading-workbook-or-worksheet/
[5]: https://docs.aspose.com/cells/java/specifying-significant-digits-to-be-stored-in-excel-file/
[6]: https://docs.aspose.com/cells/java/check-custom-number-format-when-setting-style-custom-property/
[7]: https://docs.aspose.com/cells/java/public-api-changes-in-aspose-cells-17-1-0/
[8]: https://www.aspose.com/products/cells/java
[9]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[10]: https://docs.aspose.com/cells/java
[11]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[14]: https://github.com/asposecells/Aspose_Cells_Java




