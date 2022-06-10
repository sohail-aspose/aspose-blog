---
title: 'Protect VBA Project in Excel Workbooks in Android Apps'
date: Thu, 13 Jul 2017 19:24:30 +0000
draft: false
url: /2017/07/13/protect-vba-project-in-excel-workbooks-in-android-apps/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 17.5][1]. This release includes a number of new features, enhancements and many bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a look at the most worth mentioning features in this release.

## Protect VBA Project of Excel Workbook with Password

Aspose.Cells now supports the feature of protecting the VBA (Visual Basic for Applications) Project of Excel Workbook and locking it for viewing. Besides, you can also find if the existing VBA project is already protected or locked for viewing. Please see these articles for a reference.

*   [Password Protect the VBA Project of Excel Workbook][3]
*   [Check if VBA Project is Protected and Locked for Viewing][4]
*   [Find out if VBA Project is Protected][5]

The following snippet demonstrates how to protect your Excel Workbook VBA Project dynamically using Aspose.Cells and lock it for viewing.

```
//Load your source Excel file.
Workbook wb = new Workbook(dirPath + "samplePasswordProtectVBAProject.xlsm");
  
//Access the VBA project of the workbook.
VbaProject vbaProject = wb.getVbaProject();
  
//Lock the VBA project for viewing with password.
vbaProject.protect(true, "11");
  
//Save the output Excel file.
wb.save(dirPath + "outputPasswordProtectVBAProject.xlsm");
```

## Improved Custom Load Filtering Mechanism

The LoadFilter class allows to customize the loading process as per the properties of the Worksheet. In order to customize the loading process, one has to override the LoadFilter.startSheet method. Please note, there are just a few properties that can be used for a given worksheet object in this scenario because most of the data and properties have not been loaded yet. The available Worksheet properties are: Name, Index & VisibilityType.

With the release of Aspose.Cells for Android via Java, the API has added the setter for the LoadFilter.LoadDataFilterOptions property to replace the m\_LoadDataFilterOptions instance variable. Users may change the LoadDataFilterOptions property in their own implementation of LoadFilter class to control the behavior of loading template files.

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

In order to get more in-depth understanding of the new filtering mechanism, please check the detailed article on Filtering Objects at Load Time.

## Get Paper Size of the Worksheet

Sometimes, application requirement could be to retrieve the worksheet's paper size in the unit of Inches, which can now be achieved using the PageSetup.PaperWidth and PageSetup.PaperHeight properties. The PageSetup.PaperWidth and PageSetup.PaperHeight properties are of type double representing the paper width & height in the unit of inches while considering the page orientation.

The following code snippet tries to explain the usage of PageSetup.PaperWidth and PageSetup.PaperHeight properties.

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

## Specify the Number of Significant Digits

Aspose.Cells APIs store 17 significant digits of double values unlike Excel application which stores only 15 significant digits. You can override this default behavior of Aspose.Cells APIs while using the newly exposed CellsHelper.SignificantDigits property.

The following code snippet enforces the Aspose.Cells APIs to use 15 significant digits while storing double values to the spreadsheet files of type XLSX. Please review the detailed article if you wish to get more in-depth knowledge on how to specify significant digits.

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

Aspose.Cells for Android via Java has added the CheckCustomNumberFormat property to the WorkbookSettings class. The CheckCustomNumberFormat is useful in checking if the Style.Custom property has been set properly or not. In case the Style.Custom property has been set improperly, that is; the value does not correspond to the valid pattern then the Aspose.Cells for Android via Java APIs will throw CellsException with an appropriate message.

The following code snippet tried to assign an invalid custom format to the Style.Custom property. Since the code has already set WorkbookSettings.CheckCustomNumberFormat property to true therefore the statement to set the Style.Custom property will cause CellsException.

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

## Get List of Fonts Used in Spreadsheet

Aspose.Cells for Android via Java has exposed the getFonts method for the Workbook class. The Workbook.getFonts method returns the list of individual fonts used to format the cell contents for a given spreadsheet. The list returned by the Workbook.getFonts method is in the form of an array of type com.aspose.cells.Font. 

The newly exposed method is useful in scenarios where the developers require to extract the list of the fonts used in a particular spreadsheet. The extracted list can further be used to match the available fonts on the machine before rendering the spreadsheet. This is because, if Aspose.Cells APIs are not able to find the required fonts, they try to replace the required font with some other suitable font which is present on the system. By comparing the system's font list against the fonts used in the spreadsheet, the developers can devise some mechanism to either pick the required fonts from a custom location or substitute a particular font with a list of available fonts.

The following code snippet demonstrates the usage of Workbook.getFonts method in order to [extract the list of fonts used in the sample spreadsheet][6].

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

Aspose.Cells for Android via Java has now added the HTMLLoadOptions.AutoFitColsAndRows property which indicates if the API should auto-fit columns and rows while importing the HTML in its object mode. The Boolean type property has the default value as false which means that the cell heights & widths will be imported as they are, however, when the aforementioned property is set to true, the API tries to adjust the column widths and row heights according to the contents.

The following code snippet demonstrates the usage of HTMLLoadOptions.AutoFitColsAndRows property. Please review the detailed article if you wish to get more in-depth knowledge on [how to auto fit cell contents while importing HTML in Aspose.Cells object model][7].

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

The latest revision of Aspose.Cells for Android via Java has exposed the Cells.textToColumns method in order to mimic the Excel's **Text to Columns** feature. Excel provides this feature from the command group **Data Tools** under the **Data** tab as highlighted in the following snapshot.



{{< figure align=center src="images/text-to-columns-1024x200.png" alt="Text to Columns - Excel">}}


Please note, in order to split the contents of a column to multiple columns, the data should contain a specific delimiter such as a comma (or any other character) based on which the API tries to split the contents of a cell to multiple cells.

The following code snippet demonstrates the simplest usage scenario of Cells.textToColumns method. Please review the detailed article if you wish to get more in-depth knowledge on [how to convert text to columns][8].

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

Aspose.Cells for Android via Java has exposed the WarningCallback property for the LoadOptions class in order to get or set the warning callbacks. Developers have to implement the IWarningCallback interface in order to get custom warnings in their applications.

Here is a simple usage scenario of LoadOptions.WarningCallback property to [get warnings when an input spreadsheet contains duplicate named ranges][9].

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

This revision of Aspose.Cells for Android via Java has exposed Boolean type TrimLeadingBlankRowAndColumn property for the TxtSaveOptions class that indicates whether leading blank rows and columns should be trimmed like Excel does while exporting data to CSV or Tab-delimited formats. The default value of aforementioned property is false.

In case the data on the worksheet does not start from the first cell, that is: A1, the Excel application removes the leading blank rows and columns while exporting the data to CSV or Tab-delimited formats, however, Aspose.Cells APIs by default, retain the blank rows & columns for the same sample in order to keep the data location retained if the exported CSV or Tab-delimited files have to be imported back using Aspose.Cells APIs.

Here is a simple usage scenario of TxtSaveOptions.TrimLeadingBlankRowAndColumn property. Please check the article on [trimming leading empty cells while storing contents in text formats][10] for more details.

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

## Customizing a Pivot Table by Using Globalization Settings

Using Aspose.Cells API, developers can apply various filters to build the corresponding pivot table. After they create a pivot table report and have added the fields that they require, they often want to enhance the layout and format of the report to improve readability and to make it more attractive. To achieve this, Aspose.Cells API allows developers to customize the globalization settings of a pivot table to deal with such scenarios. They can customize the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels, Blank Values text as per the requirements.

Developers can derive a class from the base GlobalizationSettings class. GlobalizationSettings class has various methods to further enhance the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels and Blank Values text. This article shows a code example which works with the layout and format of a report: [Customize Globalization Settings for Pivot Table][11].

## Specifying Sort Warning While Sorting Data

Aspose.Cells already supports Data Sorting, however earlier you could not specify that you want to sort your textual data as numerical data. For this purpose, Aspose.Cells implemented the **DataSorter.SortAsNumber** property. Whenever you sort textual data that looks like a number, MS-Excel shows this warning. **DataSorter.SortAsNumber** property implements this MS-Excel warning.



{{< figure align=center src="images/sort-textual-data-as-numbers-300x208.png" alt="">}}


Please see this article for more help relating to this topic.

*   [Specifying Sort Warning While Sorting Data][12]

## Specifying DBNum Custom Pattern Formatting

Aspose.Cells supports the **DBNum** custom pattern formatting. For example, if your cell value is **123** and you specify its custom formatting as **\[DBNum2\]\[$-804\]General** then it will be displayed like **壹佰贰拾叁**. You can specify custom formatting of your cell using Cell.getStyle() and Style.setCustom() methods.

*   [Specifying DBNum Custom Pattern Formatting][13]

## Support PDF/A-1a compliance in PdfSaveOptions

Aspose.Cells now allows you to create PDF with PDF/A-1a – Level A (accessible) conformance. It already supports PDF/A-1b – Level B (basic) conformance. Following code snippet demonstrates how to convert an Excel file to PDF compatible with PDFA-1a.

```
 //Open an Excel file.
Workbook wb = new Workbook("Book1.xlsx");
 
//Create pdf save options and set its compliance to PDFA-1a.
PdfSaveOptions opts = new PdfSaveOptions();
opts.setCompliance(PdfCompliance.PDF_A_1_A);
 
//Save the output pdf
wb.save("outputCompliancePdfA1a.pdf", opts);
```

Please see this article that explains how to convert your Excel file into PDF with PDF/A-1a conformance.

*   [Convert Excel file to PDF format compatible with PDFA-1a][14]

## Remove existing Printer Settings in Excel file

Sometimes developers want to remove existing Printer Settings in Excel file. These settings are found inside the “\[file "root"\]\\xl\\printerSettings” folder in the form of .bin files. Aspose.Cells can remove existing printer settings in the Excel workbook. For more detail, please see this article.

*   [Remove Existing PrinterSettings of Worksheets in Excel file][15]

## Implement Custom Page Size Options for the Worksheet

There is no direct option available to create custom paper sizes in MS Excel, however, you can set custom paper size of your desired worksheets when rendering Excel file to the PDF file format. This document explains how to set a custom paper size of a worksheet using Aspose.Cells APIs.

*   [Implement Custom Paper Size of Worksheet for Rendering][16]

## Shift First Row down when inserting Cells Data Table Rows

Earlier, Aspose.Cells does not shift first row down when inserting rows. But for some users' requirements, it has supported this feature now. Please see this article for more detail about this feature. It also shows an example of ICellsDataTable implementation.

*   [Export HTML String Value of the Cells to the DataTable][17]

## Copy Page Setup Settings from Source Worksheet into Destination Worksheet

When you copy worksheet into another worksheet, then page setup settings of the source worksheet are not copied to destination worksheet. Please use PageSetup.copy() method to copy the setting of the page setup from source to destination worksheet. Please see the following article for more detail.

*   [Copy Page Setup Settings from Source Worksheet into Destination Worksheet][18]

## Other Enhancements & Fixes

Aspose.Cells for Android via Java has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Ability to read the color of shape's glow effect.
*   Support for rendering gradient fill for WordArt objects while converting spreadsheets to HTML.
*   Support to load Excel 2016 chart types.

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][19].
*   [Aspose.Cells for Android via Java Download Section][20].
*   [Aspose.Cells for Android via Java Documentation][21] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][22] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][23] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][24] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][25] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/androidjava/new-releases/aspose.cells-for-android-via-java-17.5/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+17.5+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Password+Protect+the+VBA+Project+of+Excel+Workbook
[4]: https://docs.aspose.com/display/cellsjava/Check+if+VBA+Project+is+Protected+and+Locked+for+Viewing
[5]: https://docs.aspose.com/display/cellsjava/Find+out+if+VBA+Project+is+Protected
[6]: https://docs.aspose.com/display/cellsjava/Get+a+List+of+Fonts+used+in+a+Spreadsheet+or+Workbook
[7]: https://docs.aspose.com/display/cellsjava/AutoFit+Columns+and+Rows+while+loading+HTML+in+Workbook
[8]: https://docs.aspose.com/display/cellsjava/Convert+Text+to+Columns+using+Aspose.Cells
[9]: https://docs.aspose.com/display/cellsjava/Get+Warnings+while+Loading+Excel+File
[10]: https://docs.aspose.com/display/cellsjava/Trim+Leading+Blank+Rows+and+Columns+while+exporting+spreadsheets+to+CSV+format
[11]: https://docs.aspose.com/display/cellsjava/Customize+Globalization+Settings+for+Pivot+Table
[12]: https://docs.aspose.com/display/cellsjava/Specifying+Sort+Warning+While+Sorting+Data
[13]: https://docs.aspose.com/display/cellsjava/Specifying+DBNum+Custom+Pattern+Formatting
[14]: https://docs.aspose.com/display/cellsjava/Convert+Excel+file+to+PDF+format+compatible+with+PDFA-1a
[15]: https://docs.aspose.com/display/cellsjava/Remove+Existing+PrinterSettings+of+Worksheets+in+Excel+file
[16]: https://docs.aspose.com/display/cellsjava/Implement+Custom+Paper+Size+of+Worksheet+for+Rendering
[17]: https://docs.aspose.com/display/cellsjava/Shift+First+Row+down+when+inserting+Cells+Data+Table+Rows
[18]: https://docs.aspose.com/display/cellsjava/Copy+Page+Setup+Settings+from+Source+Worksheet+into+Destination+Worksheet
[19]: https://www.aspose.com/products/cells/android-java
[20]: https://downloads.aspose.com/cells/androidjava
[21]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[22]: https://apireference.aspose.com/java/cells
[23]: https://forum.aspose.com/c/cells
[24]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[25]: https://github.com/asposecells/Aspose_Cells_Java




