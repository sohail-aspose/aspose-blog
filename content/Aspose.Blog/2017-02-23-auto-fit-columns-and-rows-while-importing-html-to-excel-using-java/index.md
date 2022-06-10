---
title: 'Auto-Fit Columns and Rows while Importing HTML to Excel using Java'
date: Thu, 23 Feb 2017 13:30:35 +0000
draft: false
url: /2017/02/23/auto-fit-columns-and-rows-while-importing-html-to-excel-using-java/
author: Babar Raza
summary: ''
tags: ['Built-in Document Properties', 'CSV export', 'Excel Java API', 'HTML to Spreadsheet', 'Metered Licensing', 'Spreadsheet 2 Image', 'Spreadsheet Creation in Java', 'Template Loading', 'Text to Column', 'Waring Callback']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose team is pleased to announce the release of [Aspose.Cells for Java 17.02.0][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. The release notes also list any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java.

While you are downloading the latest build, here is a look at the biggest features from this release.

## Introducing Metered Licensing

Starting from 17.02.0 version, Aspose.Cells for Java offers the metered licensing mechanism in parallel to its traditional licensing. In order to provide the usage based licensing, Aspose.Cells for Java has exposed the Metered class that allows the developers to set public and private keys by calling its setMeteredKey method. The metered licensing system monitors the regular usage of Aspose.Cells API and keep track of the Aspose API licenses.

The following piece of code demonstrates [how to set metered public & private keys and reterieve the consumption logs][3].

```
// Set metered public and private keys
Metered metered = new Metered();
// Access the setMeteredKey property and pass public and private keys as parameters
metered.setMeteredKey("************", "************");
// Instantiate a new Workbook object
Workbook workbook = new Workbook();
// Check if the license is set
System.out.println(workbook.isLicensed());
  
  
// Get the Consumption quantity
double amountBefore = Metered.getConsumptionQuantity();
System.out.println(amountBefore);
Workbook workbook2 = new Workbook(dir + "sample.xlsx");
workbook2.save("out1.xlsx");
// Get the Consumption quantity again which should be greater a bit
double amountAfter = Metered.getConsumptionQuantity();
System.out.println(amountAfter); 
```

## Get List of Fonts Used in Spreadsheet

Aspose.Cells for Java 17.02.0 has exposed the getFonts method for the Workbook class. The Workbook.getFonts method returns the list of individual fonts used to format the cell contents for a given spreadsheet. The list returned by the Workbook.getFonts method is in the form of an array of type com.aspose.cells.Font. 

The newly exposed method is useful in scenarios where the developers require to extract the list of the fonts used in a particular spreadsheet. The extracted list can further be used to match the available fonts on the machine before rendering the spreadsheet. This is because, if Aspose.Cells APIs are not able to find the required fonts, they try to replace the required font with some other suitable font which is present on the system. By comparing the system's font list against the fonts used in the spreadsheet, the developers can devise some mechanism to either pick the required fonts from a custom location or substitute a particular font with a list of available fonts.

Following code snippet demonstrates the usage of Workbook.getFonts method in order to [extract the list of fonts used in the sample spreadsheet][4].

```
// Create an instance of Workbook and load a sample
Workbook book = new Workbook(dir + "sample.xlsx");
 
// Retrieve the list of fonts used in spreadsheet
Font[] fonts = book.getFonts();
 
// Iterate the list and write font name
for (int i = 0; i < fonts.length; i ++)
{
    Font font = fonts[i];
    System.out.println(font.getName());
} 
```

## Auto-Fit Columns and Rows while Importing HTML

Aspose.Cells for Java has now added the HTMLLoadOptions.AutoFitColsAndRows property which indicates if the API should auto-fit columns and rows while importing the HTML in its object mode. The Boolean type property has the default value as false which means that the cell heights & widths will be imported as they are, however, when the aforementioned property is set to true, the API tries to adjust the column widths and row heights according to the contents.

The following code snippet demonstrates the usage of HTMLLoadOptions.AutoFitColsAndRows property. Please review the detailed article if you wish to get more in-depth knowledge on [how to auto fit cell contents while importing HTML in Aspose.Cells object model][5].

```
// Create an instance of HTMLLoadOptions
HTMLLoadOptions loadOptions = new HTMLLoadOptions();
 
// Set the AutoFitColsAndRows property to true
loadOptions.setAutoFitColsAndRows(true);
 
// Create an instance of Workbook and load HTML while passing
// the object of HTMLLoadOptions class created above
Workbook book = new Workbook(dir + "sample.htm", loadOptions); 
```

## Convert Text to Columns

Latest revision of Aspose.Cells for Java has exposed the Cells.textToColumns method in order to mimic the Excel's **Text to Columns** feature. Excel provides this feature from the command group **Data Tools** under the **Data** tab as highlighted in the following snapshot.



{{< figure align=center src="images/text-to-columns-1024x200.png" alt="Text to Columns - Excel">}}


Please note, in order to split the contents of a column to multiple columns, the data should contain a specific delimiter such as a comma (or any other character) based on which the API tries to split the contents of a cell to multiple cells.

The following code snippet demonstrates the simplest usage scenario of Cells.textToColumns method. Please review the detailed article if you wish to get more in-depth knowledge on [how to convert text to columns][6].

```
// Create an instance of Workbook and load a sample
Workbook book = new Workbook(dir + "sample.xlsx");
 
// Retrieve the cells collection of the first worksheet in the sample
Cells cells = book.getWorksheets().get(0).getCells();
 
// Create an instance of TxtLoadOptions
TxtLoadOptions options = new TxtLoadOptions();
 
// Specify the separator
options.setSeparator(',');
 
// Split the data in range B2:B4
cells.textToColumns(1, 1, 3, options); 
```

## Warning Callback for Template Loading

Aspose.Cells for Java 17.02.0 has exposed the WarningCallback property for the LoadOptions class in order to get or set the warning callbacks. Developers have to implement the IWarningCallback interface in order to get custom warnings in their applications.

Here is a simple usage scenario of LoadOptions.WarningCallback property to [get warnings when an input spreadsheet contains duplicate named ranges][7].

```
public class WarningCallback implements IWarningCallback
{
    public void warning(WarningInfo warningInfo)
    {
        if (warningInfo.getWarningType() == WarningType.DUPLICATE_DEFINED_NAME)
        {
            System.out.println("Duplicate Defined Names Found as " + warningInfo.getDescription());
        }
    }
} 
```

Here is how to use the custom class defined above.

```
// Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();
 
// Set the WarningCallback property to custom class
options.setWarningCallback(new WarningCallback());
 
// Load a sample spreadsheet in an instance of Workbook while 
// passing the object of LoadOptions class as defined above
Workbook book = new Workbook(dir + "sample.xlsx", options); 
```

## Trim Leading Blank Rows & Columns while Exporting Contents to Text Formats

This revision of Aspose.Cells for Java has exposed Boolean type TrimLeadingBlankRowAndColumn property for the TxtSaveOptions class that indicates whether leading blank rows and columns should be trimmed like Excel does while exporting data to CSV or Tab-delimited formats. The default value of aforementioned property is false.

In case the data on the worksheet does not start from the first cell, that is: A1, the Excel application removes the leading blank rows and columns while exporting the data to CSV or Tab-delimited formats, however, Aspose.Cells APIs by default, retain the blank rows & columns for the same sample in order to keep the data location retained if the exported CSV or Tab-delimited files have to be imported back using Aspose.Cells APIs.

Here is a simple usage scenario of TxtSaveOptions.TrimLeadingBlankRowAndColumn property. Please check the article on [trimming leading empty cells while storing contents in text formats][8] for more details.

```
// Create an instance of Workbook and load a sample
Workbook book = new Workbook(dir + "sample.xlsx");
 
// Create an instance of TxtSaveOptions
TxtSaveOptions options = new TxtSaveOptions();
 
// Set TrimLeadingBlankRowAndColumn property to true
options.setTrimLeadingBlankRowAndColumn(true);
 
// Export to CSV format while removing the leading blank rows & columns
book.save(dir + "output.csv", options); 
```

## Other Enhancements & Fixes

Aspose.Cells for Java 17.02.0 has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Support to [load Excel 2016 chart types][9].
*   Enhanced HTML rendering engine for shapes.
*   Handled a few exceptions such as NullPointerException & IndexOutOfBoundsException.

## Changes to the Public API

This revision of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   The BuiltInDocumentPropertyCollection.RevisionNumber property has been replaced by the BuiltInDocumentPropertyCollection.Revision property.
*   Added Shape.TextShapeType property that gets or sets the preset text shape type from a list of predefined types stored in AutoShapeType enumeration.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][10].
*   [Aspose.Cells for Java Download Section][11].
*   [Aspose.Cells for Java Documentation][12] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][15] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.02.0/
[2]: https://docs.aspose.com/cells/java/
[3]: https://docs.aspose.com/cells/java/licensing/#Licensing-ApplyingMeteredLicense
[4]: https://docs.aspose.com/cells/java/get-a-list-of-fonts-used-in-a-spreadsheet-or-workbook/
[5]: https://docs.aspose.com/cells/java/autofit-columns-and-rows-while-loading-html-in-workbook/
[6]: https://docs.aspose.com/cells/java/convert-text-to-columns-using-aspose-cells/
[7]: https://docs.aspose.com/cells/java/get-warnings-while-loading-excel-file/
[8]: https://docs.aspose.com/cells/java/trim-leading-blank-rows-and-columns-while-exporting-spreadsheets-to-csv-format/
[9]: https://docs.aspose.com/cells/java/read-and-manipulate-excel-2016-charts/
[10]: https://products.aspose.com/cells/java
[11]: https://downloads.aspose.com/cells/java
[12]: https://docs.aspose.com/cells/java
[13]: https://apireference.aspose.com/cells/java
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[16]: https://github.com/asposecells/Aspose_Cells_Java




