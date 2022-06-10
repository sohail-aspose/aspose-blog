---
title: 'Impose Excel 2003 Restrictions while Refreshing Pivot Tables using Java'
date: Mon, 25 Jul 2016 11:31:13 +0000
draft: false
url: /2016/07/25/impose-excel-2003-restrictions-while-refreshing-pivot-tables-using-java/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 8.9.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Impose Restrictions of Excel 2003 while Refreshing Pivot Table

Aspose.Cells for Java API has exposed the Boolean type IsExcel2003Compatible property for the PivotTable class which allows to impose or remove the Excel 2003 restrictions for refreshing Pivot Tables. The default value of IsExcel2003Compatible property is true, that means a string must be less than or equal to 255 characters. If the string is greater than 255 characters, it will be truncated. If false, the aforementioned restriction will not be imposed.

Below provided code snippet demonstrates the simple usage scenario of PivotTable.IsExcel2003Compatible property. In order to get a more detailed understanding of this feature, please check the article on Compatibility for Excel 2003 while Refreshing Pivot Tables.

```
//Load a spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");

//Access the desired Pivot Table from the spreadsheet
PivotTable pivot = book.getWorksheets().get(0).getPivotTables().get(0);

//Set Excel 2003 compatibility to false
pivot.setExcel2003Compatible(false);

//Refresh & recalculate Pivot Table
pivot.refreshData();
pivot.calculateData();
```

## Set Default Font for Rendering Spreadsheets to Image Formats

Aspose.Cells for Java API has provided the ability to specify the default font name for rendering the spreadsheets in image formats by exposing the ImageOrPrintOptions.DefaultFont property. The DefaultFont property is of type System.string with default value as null. The said property can be used when Unicode characters in the spreadsheet have not been formatted with appropriate font in the cell's style, consequently, such characters may appear as blocks in the resultant images. It is advised to set the DefaultFont property to MingLiu or MS Gothic to properly show the Unicode characters in the resultant images. If the DefaultFont property is not set, Aspose.Cells for Java API will use the system's default font to show the Unicode characters.

Below provided code snippet demonstrates the simple usage scenario of newly exposed ImageOrPrintOptions.DefaultFont property. Please check the detailed article on Setting Default Font for Rendering Spreadsheets in Image Formats if you wish to get more in-depth understanding of the aforementioned feature.

```
//Create an instance of ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions();
//Set default font name for image rendering
options.setDefaultFont("MS Gothic");

//Load a spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");
//Access the worksheet to be rendered
Worksheet sheet = book.getWorksheets().get(0);

//Create an instance of SheetRender
SheetRender render = new SheetRender(sheet, options);
//Save spreadsheet to image
render.toImage(0, dir + "output.png");
```

## Set Default Font for Rendering Spreadsheets to HTML

Aspose.Cells for Java 8.9.0 has exposed the DefaultFontName property for the HtmlSaveOptions class that allows to specify the default font name while rendering spreadsheets to HTML format. The default font will be used only when a particular font used to style some contents in the spreadsheet does not exist on the machine where conversion process has to take place. The default value of HtmlSaveOptions.DefaultFontName property is null that means, Aspose.Cells for Java API will use the universal font which has the same family with the original font.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.DefaultFontName. In order to get a more in-depth  understanding of this feature, please check the article on Setting Default Font for Rendering Spreadsheets to HTML Format.

```
//Create an instance of HtmlSaveOptions
HtmlSaveOptions options = new HtmlSaveOptions();
//Set default font name for Html rendering
options.setDefaultFontName("Arial");

//Load a spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");
//Save the spreadsheet in Html format while passing instance of HtmlSaveOptions
book.save(dir + "output.html", options);
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Expanding text from right to left while exporting spreadsheets to HTML.
*   Improved SheetRender for controls such as CheckBox.
*   Handled a few critical exceptions.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][2].
*   [Aspose.Cells for Java Download Section][3].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][4] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][6] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cells/java/new-releases/aspose.cells-for-java-8.9.0/
[2]: http://www.aspose.com/java/excel-component.aspx
[3]: https://downloads.aspose.com/cells/java
[4]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[5]: https://forum.aspose.com/
[6]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[7]: https://github.com/asposecells/Aspose_Cells_Java




