---
title: 'Change Worksheet cells Alignment in Excel within Android Apps'
date: Mon, 08 Oct 2018 18:27:04 +0000
draft: false
url: /2018/10/08/change-worksheet-cells-alignment-encrypt-or-decrypt-ods-files-and-export-custom-document-properties-to-pdf-using-aspose.cells-for-android-via-java-18.9/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100-e1539021448359.png" alt="">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 18.9][1]. This release includes some new features, enhancements and other bug fixes that further improve the overall stability and usability of the API. For an easy access and utilization, Aspose.Cells for Android via Java APIs can be directly installed from Maven repository, see the [document][2] for your reference. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a quick look at the most worth mentioning features in this release.

## Change Cells Alignment and Keep Existing Formatting

It is quite often that we need to change the alignment of multiple cells but at the same time need to maintain the existing formatting as well. **StyleFlag.Alignments** property is provided by Aspose.Cells to achieve this functionality. Please note, **StyleFlag** object is passed as a parameter to **Range.applyStyle()** method which actually applies the formatting to your desired range of cells. The following sample code loads the sample Excel file, creates the range and center aligns it horizontally and vertically and keeps the existing formatting intact.

```
// Load sample Excel file containing cells with formatting.Workbook wb = new Workbook(dirPath + "sampleChangeCellsAlignmentAndKeepExistingFormatting.xlsx");// Access first worksheet.Worksheet ws = wb.getWorksheets().get(0);// Create cells range.Range rng = ws.getCells().createRange("B2:D7");// Create style object.Style st = wb.createStyle();// Set the horizontal and vertical alignment to center.st.setHorizontalAlignment(TextAlignmentType.CENTER);st.setVerticalAlignment(TextAlignmentType.CENTER);// Create style flag object.StyleFlag flag = new StyleFlag();// Set style flag alignments true. It is most crucial statement.// Because if it will be false, no changes will take place.flag.setAlignments(true);// Apply style to range of cells.rng.applyStyle(st, flag);// Save the workbook in XLSX format.wb.save(dirPath + "outputChangeCellsAlignmentAndKeepExistingFormatting.xlsx", SaveFormat.XLSX); 
```

Please see the following article for more detail on this topic for your reference.

*   [Change Cells Alignment and Keep Existing Formatting][4]

## Find Maximum Rows and Columns supported by XLS and XLSX formats

For your information, there are different number of rows and columns supported by different MS Excel file formats. For example, XLS supports up to 65536 rows and 256 columns while XLSX supports 1048576 rows and 16384 columns. If you want to know how many rows and columns are supported by a given format, you can use **Workbook.getSettings().getMaxRow()** and **Workbook.getSettings().getMaxColumn()** methods. Please see the following article for more detail on this topic for your reference:  

*   [Find Maximum Rows and Columns supported by XLS and XLSX formats][5]

## Specify Author while Write Protecting Workbook

You can specify author name while write protecting your workbook using Aspose.Cells API. Please use **Workbook.getSettings().getWriteProtection().setAuthor()** method for this purpose. Please see the following article for more detail on this topic for your reference:

*   [Specify Author while Write Protecting Workbook][6]

## Encrypt/decrypt an ODS file

Aspose.Cells allows you to encrypt and decrypt an ODS file. Decrypted ODS file can be opened both in MS Excel and OpenOffice, however encrypted ODS file can only be opened by OpenOffice after providing the password. Excel cannot open the encrypted ODS file and may raise warning message. For encrypting an ODS file, load the file and set the **WorkbookSettings.Password** value to the actual password before saving it. Please see the following article for more detail on this topic for your reference:

**Encrypt ODS File**

```
// Open an ODS fileWorkbook workbook = null;workbook = new Workbook(dirPath + "Book1.ods");// Password protect the fileworkbook.getSettings().setPassword("1234");// Save the ODS fileworkbook.save(dirPath + "encryptedBook1.out.Java.ods");
```

**Decrypt ODS File**

```
// Open an encrypted ODS fileLoadOptions loadOptions = new LoadOptions(LoadFormat.ODS);// Set original passwordloadOptions.setPassword("1234");// Load the encrypted ODS file with the appropriate load optionsWorkbook workbook = null;workbook = new Workbook(dirPath + "encryptedBook1.out.Java.ods", loadOptions);// Unprotect the workbookworkbook.unprotect("1234");// Set the password to nullworkbook.getSettings().setPassword(null);// Save the decrypted ODS fileworkbook.save(dirPath + "DencryptedBook1.out.Java.ods");
```

## Applying text alignment to partial text inside the TextBox

It is very common to apply different alignments to the partial texts in the text box. This feature was having some issues but now it is reviewed and bugs are removed to incorporate proper alignment.     

For a working example refer to the following article:

*   [Applying text alignment to partial text inside the Textbox][7]  

## Content Copying for accessibility

This option allows screen reader software to utilize the text within the PDF file for reading.  You can disable it by applying a change permissions password and deselecting few options in Adobe Acrobat. Same functionality can be achieved  using Aspose.Cells for Java now.   

For a working example refer to the following article:

*   [Set content copy for accessibility option][8] 

## Disable Pivot Table Ribbon 

Pivot table based reports are useful but prone to error if target users do not have detailed knowledge of Excel to configure these reports. In these circumstances organizations will want to restrict users from being able to change a pivot table based report. Common pivot table features like adding additional filters, slicers, fields, or changing the order of certain things in the report are mostly not recommended for every user. On the other hand, these users shall also be able to refresh the report and use existing filters or slicers. Aspose.Cells has provided this ability to developers for restricting users from changing these reports while creating them. For this purpose Excel provides feature to disable pivot table ribbon and same is provided by Aspose.Cells i.e. developer can disable the ribbon which contain controls to modify these reports.

For a working example along with a template file refer to the following article:

*   [Disable Pivot Table Ribbon][9]

## Improvements in process interruption 

Reliability and efficiency is basic requirement by the users for any software product. If some conversion takes too long, sometimes it is required to interrupt this process to return control to the user. This feature is already present but got some performance issues, however we have further improved it and now can be used without any trouble.    

For a working example refer to the following article:

*   [Aspose.Cells for Java - Interruptible Library][10] 

## Pasting rows/columns with paste option 

While working with Excel, pasting rows and columns is very common and this feature was introduced in the earliest versions of Aspose.Cells. However limited paste option was available in contrast to Excel where variety of options are available when we paste data somewhere in Excel. Now Aspose.Cells has provided this feature and you can paste data with multiple options.     

For a working example refer to the following article:

*   [Pasting rows and columns with paste options][11] 

## Export custom document properties to PDF

Many documents can have custom properties which were not made part of the PDFs earlier. Now we have provided this feature to maintain the precious information through custom properties by exporting them to the PDF files. These properties can be observed in Adobe Acrobat Reader by clicking on File and then Custom tab page in properties sheet.     

For a working example refer to the following article:

*   [Export custom document properties to PDF][12]

## Get XML path from List Object/Table

XML data can be imported to worksheets where sometimes XML path is required from the ListObjects of the worksheet. This feature is available in Excel by using expression like Sheet1.ListObjects(1).XmlMap.DataBinding. We are glad to share that this feature is available now in Aspose.Cells as well.   

For a working example refer to the following article:

*   [Get XML path from ListObject/Table][13]  

## Create safe sheet names 

Sometimes there is a need of assigning the sheet name at runtime. In this scenario, there may be sheet names which may contain some additional characters like <>+(?”. There is a need to replace any such character, which is not allowed as a sheet name with some preset character provided by user. Similarly the length may increase to more than 31 characters which needs to be truncated. Apache POI provides certain features of creating safe names, hence similar feature is provided by Aspose.Cells to handle all these issues.

For a working example along with a template file refer to the following article:

*   [Create safe sheet names similar to Apache POI][14]

## Enhanced filters like Contains, Not Contains, Blank and Non-Blank 

We have increased the range of auto filters like filtering based on fill color, date, dynamic date, number and texts. These filters were already part of our previous releases. Need was felt to add filters like blank/non-blank and custom filters with contains and not-contains. This time these filters are added along with sample files so that these features can be tested easily.   

For a working example refer to the following article:

*   [Filtering with Blanks/Non-Blanks and custom contains/Not-Contains][15] 

## Retrieve query table result range 

QueryTable represents a worksheet table built from data returned from an external data source, such as an sql server or a Microsoft access database.  Aspose.Cells provides option to read the address i.e. result range of cells for a query table.    

For a working example refer to the following article:

*   [Retrieve range of query table][16] 

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][17].
*   [Aspose.Cells for Android via Java Download Section][18].
*   [Aspose.Cells for Android via Java Documentation][19] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][20] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][21] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][22] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][23] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.9/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+Installation#Aspose.CellsforAndroidviaJavaInstallation-InstallAspose.CellsforAndroidviaJavafromMavenRepository
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+18.6+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Change+Cells+Alignment+and+Keep+Existing+Formatting
[5]: https://docs.aspose.com/display/cellsjava/Find+Maximum+Rows+and+Columns+supported+by+XLS+and+XLSX+formats
[6]: https://docs.aspose.com/display/cellsjava/Specify+Author+while+Write+Protecting+Workbook
[7]: https://docs.aspose.com/display/cellsjava/Applying+text+alignment+to+partial+text+inside+the+TextBox
[8]: https://docs.aspose.com/display/cellsjava/Saving+Excel+files+to+CSV%2C+PDF+and+other+formats#SavingExcelfilestoCSV,PDFandotherformats-SetContentCopyForAccessibilityoption
[9]: https://docs.aspose.com/display/cellsjava/Disable+Pivot+Table+Ribbons
[10]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+-+Interruptible+Library
[11]: https://docs.aspose.com/display/cellsjava/Copying+Rows+and+Columns#CopyingRowsandColumns-PastingRows/ColumnswithPasteOptions
[12]: https://docs.aspose.com/display/cellsjava/Saving+Excel+files+to+CSV%2C+PDF+and+other+formats#SavingExcelfilestoCSV,PDFandotherformats-ExportCustompropertiestoPDF
[13]: https://docs.aspose.com/display/cellsjava/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method#QueryCellAreasMappedtoXmlMapPathusingWorksheet.XmlMapQuerymethod-GetXMLpathfromListObject/Table
[14]: https://docs.aspose.com/display/cellsjava/Names+and+Indices#NamesandIndices-Createsafesheetnames
[15]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-Blanks
[16]: https://docs.aspose.com/display/cellsjava/Reading+and+Writing+Query+Table+of+Worksheet
[17]: https://www.aspose.com/products/cells/android-java
[18]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.6/
[19]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[20]: https://apireference.aspose.com/java/cells
[21]: https://forum.aspose.com/c/cells
[22]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[23]: https://github.com/asposecells/Aspose_Cells_Java




