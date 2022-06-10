---
title: 'Load Visible Worksheets Only using Java with Aspose.Cells for Java 8.6.3'
date: Mon, 04 Jan 2016 12:49:01 +0000
draft: false
url: /2016/01/04/load-only-visible-worksheets-create-excels-built-in-styles-with-aspose.cells-for-java-8.6.3/
author: Babar Raza
summary: ''
tags: ['API to Convert Spreadsheets', 'API to Create Spreadsheets', 'Babar Raza', 'Excel Java APIs', 'Excel file', 'Worksheet', 'spreadsheet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose.Cells for Java API has been upgraded to 8.6.3, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.6.3][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Load Only Visible Worksheets from Existing Spreadsheet

Aspose.Cells APIs provide a set of classes for the developers to influence the spreadsheet loading mechanism. While using the LoadOptions & LoadDataOptions classes, the developers can set a number of options such as force the API to load specific worksheets, where the worksheets can be specified via their indices or names.

Aspose.Cells for Java 8.6.3 has exposed another useful property for the LoadDataOptions class which allows loading only the visible worksheets from an existing spreadsheet, where the hidden worksheets will be simply ignored and will not be available in the Aspose.Cells object model for any processing. The newly exposed property LoadDataOptions.OnlyVisibleWorksheet is of type Boolean; setting it to true means that the API will ignore the hidden worksheets and load only the visible worksheets for further processing.

The following piece of code demonstrates the usage of LoadDataOptions.OnlyVisibleWorksheet property to load only visible worksheets.

```
//Create an instance of LoadDataOption
LoadDataOption loadDataOptions = new LoadDataOption();

//Set OnlyVisibleWorksheet property to true
loadDataOptions.setOnlyVisibleWorksheet(true);

//Create an instance of LoadOptions
LoadOptions loadOptions = new LoadOptions();

//Set LoadDataOptions property to the instance of LoadDataOption created earlier
loadOptions.setLoadDataOptions(loadDataOptions);

//Create an instance of Workbook & load an existing spreadsheet
//while passing the instance of LoadOptions created earlier
Workbook book = new Workbook(inputFilePath, loadOptions);
```

## Create Excel's Built-in Styles

Aspose.Cells for Java 8.6.3 has exposed the Workbook.createBuiltinStyle method that can be used to create an object of the Style class that corresponds to one of the built-in styles offered by the Excel application. The Workbook.createBuiltinStyle method accepts a constant from the enumeration BuiltinStyleType.

Please note, with previous releases of the Aspose.Cells APIs, same task could be accomplished via StyleCollection.createBuiltinStyle method but as the recent releases of Aspose.Cells APIs have removed the StyleCollection class from the public API therefore the newly exposed Workbook.createBuiltinStyle method can be considered as an alternative approach to achieve the same goal.

The following sample code explains how to [create Excel's built-in styles][3].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-UsingBuiltinStyles-UsingBuiltinStyles.java" >}}

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Aspose.Cells for Java 8.6.3 has exposed the ImportTableOptions.setHtmlString attribute which directs the API to parse the HTML tags while importing data onto the Worksheet and set the parsed result as cell value. Please note, Aspose.Cells APIs already provide the Cell.setHtmlString attribute to perform this task for a single cell, however, while importing data in bulk, the ImportTableOptions.setHtmlString attribute (when set to true) tries to parse all the supported HTML tags and sets the parsed results to the corresponding cells.
*   This release has addressed some formatting issues reported for the XML Spreadsheet 2003 to XLSX conversion.
*   Enhanced the PDF rending engine to maximize the fidelity for the Excel Chart objects.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Cells for Java API][4].
*   [Download Aspose.Cells for Java][5].
*   [Aspose.Cells for Java online documentation][6] – help documentation and API reference documents.
*   [Aspose.Cells Product Family Forum][7] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes, and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: http://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Using+Built-in+Styles
[4]: https://products.aspose.com/cells/java
[5]: https://downloads.aspose.com/cells/java
[6]: http://docs.aspose.com/display/cellsjava/home
[7]: https://forum.aspose.com/
[8]: https://blog.aspose.com/
[9]: https://github.com/asposecells/Aspose_Cells_Java




