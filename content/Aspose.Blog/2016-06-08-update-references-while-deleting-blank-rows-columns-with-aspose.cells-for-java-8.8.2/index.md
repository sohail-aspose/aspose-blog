---
title: 'Update References while Deleting Blank Rows &amp; Columns with Aspose.Cells for Java 8.8.2'
date: Wed, 08 Jun 2016 10:40:24 +0000
draft: false
url: /2016/06/08/update-references-while-deleting-blank-rows-columns-with-aspose.cells-for-java-8.8.2/
author: Babar Raza
summary: ''
tags: ['Delete Blank Rows Columns', 'Delete Blank Rows and Columns in Excel', 'Java Spreadsheet APIs', 'Remove empty rows and columns in Excel', 'Update Cell References']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 8.8.2][1]. This release includes some new features, enhancements and bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Deleting Blank Rows & Columns with Updated References

As per default behaviour, Aspose.Cells APIs delete the blank rows & columns without updating the cell references that may have been effected from the delete process. This could lead to undesired results in certain cases, especially when spreadsheet contains formulas or charts.

Aspose.Cells APIs have tried to overcome the aforementioned situation by exposing the overloaded versions of the _Cells.deleteBlankRows_ & _Cells.deleteBlankColumns_ methods with the release of Aspose.Cells for Java 8.8.2. The new methods can accept an instance of DeleteOptions class and can be used to overcome the situations that could arise due to the broken references in formulas, chart series data and so on. The DeleteOptions class currently has one member, a Boolean type property by the name UpdateReference. If the said property is set to true and the instance of DeleteOptions class is passed to the _Cells.deleteBlankRows_ & _Cells.deleteBlankColumns_ methods, the API will internally adjust the formula references (if any) to accommodate the changes.

Below provided code snippet demonstrates the simple usage scenario of newly exposed overloads. If you wish to get more understanding where these methods should be used, please check the detailed article on [updating cell references while deleting blank rows & columns][4].

```
//Create an instance of Workbook & load an existing spreadsheet
Workbook book = new Workbook(dir + "sample.xlsx");

//Access worksheet from which blank rows/columns have to be deleted
Worksheet sheet = book.getWorksheets().get(0);

//Access cells of the desired worksheet
Cells cells = sheet.getCells();

//Create an instance of DeleteOptions class
DeleteOptions options = new DeleteOptions();
//Set UpdateReference property to true;
options.setUpdateReference(true);

//Delete all blank rows and columns
cells.deleteBlankColumns(options);
cells.deleteBlankRows(options);
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Ability to [render Unicode Supplementary Characters in PDF][5].
*   Enhanced Chart2Image feature for data labels.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][6].
*   [Aspose.Cells for Java Download Section][7].
*   [Aspose.Cells for Java Documentation][8] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][9] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][10] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][11] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][12] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: http://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+8.8.2+Release+Notes
[3]: http://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: http://docs.aspose.com/display/cellsjava/Update+references+in+other+worksheets+while+deleting+blank+columns+and+rows+in+a+worksheet
[5]: http://docs.aspose.com/display/cellsjava/Render+Unicode+Supplementary+characters+in+output+Pdf+by+Aspose.Cells
[6]: https://products.aspose.com/cells/java
[7]: https://downloads.aspose.com/cells/java
[8]: http://docs.aspose.com/display/cellsjava/home
[9]: https://apireference.aspose.com/java/cells/
[10]: https://forum.aspose.com/c/cells
[11]: https://blog.aspose.com/
[12]: https://github.com/aspose-cells/Aspose.Cells-for-Java




