---
title: 'Maintain Formatting while Changing Cell Alignment and Encrypt or Decrypt ODS Files using Aspose.Cells for Java 18.7'
date: Fri, 27 Jul 2018 17:04:01 +0000
draft: false
url: /2018/07/27/maintain-formatting-while-changing-cells-alignment-and-encrypt-or-decrypt-ods-files-using-aspose.cells-for-java-18.7/
author: Ahsaniqbal
summary: ''
tags: ['Encrypt or decrypt ODS spreadsheets in Java', 'change cell alignment in Excel in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


It is a pleasure for us to announce the release of **Aspose.Cells for Java v18.7** with a lot of new utility features that are added for common users. Important fixes and other enhancements are also part of this new release. For detailed information about this release, visit the [release notes][1] providing details about the enhancements, bugs which are fixed and handling of a variety of exceptions. For easy access and utilization, Aspose for Java APIs can be directly installed from Maven repository for which please check the [document][2].  

## Change Cells Alignment and Keep Existing Formatting

It is quite often that we need to change the alignment of multiple cells but at the same time need to maintain the existing formatting as well. **StyleFlag.Alignments** property is provided by Aspose.Cells to achieve this functionality. Please note, **StyleFlag** object is passed as a parameter to **Range.applyStyle()** method which actually applies the formatting to your desired range of cells. The following sample code loads the sample Excel file, creates the range and center aligns it horizontally and vertically and keeps the existing formatting intact.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Data-ChangeCellsAlignmentAndKeepExistingFormatting.java" >}}

```
// Load sample Excel file containing cells with formatting.Workbook wb = new Workbook("sampleChangeCellsAlignmentAndKeepExistingFormatting.xlsx");// Access first worksheet.Worksheet ws = wb.getWorksheets().get(0);// Create cells range.Range rng = ws.getCells().createRange("B2:D7");// Create style object.Style st = wb.createStyle();// Set the horizontal and vertical alignment to center.st.setHorizontalAlignment(TextAlignmentType.CENTER);st.setVerticalAlignment(TextAlignmentType.CENTER);// Create style flag object.StyleFlag flag = new StyleFlag();// Set style flag alignments true. It is most crucial statement.// Because if it will be false, no changes will take place.flag.setAlignments(true);// Apply style to range of cells.rng.applyStyle(st, flag);// Save the workbook in XLSX format.wb.save("outputChangeCellsAlignmentAndKeepExistingFormatting.xlsx", SaveFormat.XLSX);
```

Please see the following article for more detail on this topic for your reference.

*   [Change Cells Alignment and Keep Existing Formatting][3]

## Find Maximum Rows and Columns supported by XLS and XLSX formats

For your information, there are a different number of rows and columns supported by different MS Excel file formats. For example, XLS supports up to 65536 rows and 256 columns while XLSX supports 1048576 rows and 16384 columns. If you want to know how many rows and columns are supported by a given format, you can use **Workbook.getSettings().getMaxRow()** and **Workbook.getSettings().getMaxColumn()** methods. Please see the following article for more detail on this topic for your reference:  

*   [Find Maximum Rows and Columns supported by XLS and XLSX formats][4]

## Specify Author while Write Protecting Workbook

You can specify author name while write protecting your workbook using Aspose.Cells API. Please use **Workbook.getSettings().getWriteProtection().setAuthor()** method for this purpose. Please see the following article for more detail on this topic for your reference:

*   [Specify Author while Write Protecting Workbook][5]

## Encrypt/decrypt an ODS file

Aspose.Cells allows you to encrypt and decrypt an ODS file. Decrypted ODS file can be opened both in MS Excel and OpenOffice, however, encrypted ODS file can only be opened by OpenOffice after providing the password. Excel cannot open the encrypted ODS file and may raise warning messages. For encrypting an ODS file, load the file and set the **WorkbookSettings.Password** value to the actual password before saving it. Please see the following article for more detail on this topic for your reference:

**Encrypt ODS File**

```
// Open an ODS fileWorkbook workbook = null;workbook = new Workbook("Book1.ods");// Password protect the fileworkbook.getSettings().setPassword("1234");// Save the ODS fileworkbook.save("encryptedBook1.out.Java.ods");
```

**Decrypt ODS File**

```
// Open an encrypted ODS fileLoadOptions loadOptions = new LoadOptions(LoadFormat.ODS);// Set original passwordloadOptions.setPassword("1234");// Load the encrypted ODS file with the appropriate load optionsWorkbook workbook = null;workbook = new Workbook("encryptedBook1.out.Java.ods", loadOptions);// Unprotect the workbookworkbook.unprotect("1234");// Set the password to nullworkbook.getSettings().setPassword(null);// Save the decrypted ODS fileworkbook.save("DencryptedBook1.out.Java.ods");
```

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Support multiple values when using class style
*   Correction in Smart Art Image extraction
*   Resolve hyperlinks issue when viewing the output Excel file in MS Excel Japanese version
*   Handled "Getting #NUM for a cell having IRR function"
*   HTML to XLS - CSS style ignored
*   Handled  "java.lang.NumberFormatException" while loading an Excel file
*   Handled "java.lang.NullPointerException" while calculating formula

In Aspose.Cells 18.7, we fixed several important bugs and other issues. For example, issues around Workbooks with XL4 macros (XLSM), fetching comment text instead of alternative text, handling exceptions like "IndexOutOfBoundsException" while calling Chart.calculate() and "Invalid encoding: null" while loading the XLS file. Similarly, features are added to [Change Cells Alignment and Keep Existing Formatting][6], [Find Maximum Rows and Columns supported by XLS and XLSX formats][7] and [Specify Author while Write Protecting Workbook][8].

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **enum StyleFlag.Alignments**, it represents all the settings of alignment.
*   Adds **WorkbookSettings.MaxRow** and **WorkbookSettings.MaxColumn** properties, these attributes gets the max row and column indexes of the workbook.
*   Adds **WriteProtection.Author** property, it gets and sets the author of the write protection.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Download Aspose.Cells for Java][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.7+Release+Notes
[2]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[3]: https://docs.aspose.com/display/cellsjava/Change+Cells+Alignment+and+Keep+Existing+Formatting
[4]: https://docs.aspose.com/display/cellsjava/Find+Maximum+Rows+and+Columns+supported+by+XLS+and+XLSX+formats
[5]: https://docs.aspose.com/display/cellsjava/Specify+Author+while+Write+Protecting+Workbook
[6]: https://docs.aspose.com/display/cellsjava/Change+Cells+Alignment+and+Keep+Existing+Formatting
[7]: https://docs.aspose.com/display/cellsjava/Find+Maximum+Rows+and+Columns+supported+by+XLS+and+XLSX+formats
[8]: https://docs.aspose.com/display/cellsjava/Specify+Author+while+Write+Protecting+Workbook
[9]: https://products.aspose.com/cells/java
[10]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java




