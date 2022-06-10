---
title: 'Assign Macros to Controls or Shapes in Excel Spreadsheets using Java'
date: Wed, 30 Sep 2015 07:29:14 +0000
draft: false
url: /2015/09/30/assign-macros-to-controls-or-shapes-in-excel-in-java/
author: Babar Raza
summary: ''
tags: ['Assign macros to shapes in Excel', 'Babar Raza', 'Spreadsheet Metadata', 'VBA Modules']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose.Cells for Java API has been upgraded to 8.6.0, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.6.0][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Assign Macros to Shapes in Excel

Aspose.Cells for Java now provides the Shape.MarcoName property to [assign the macros to any control in the spreadsheet][3]. This property is useful in scenarios where the application requirement is to add modules and assign them to the controls for user interaction.

The following sample code explains the usage of Shape.MarcoName property to assign a simple newly added module to button click event.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-AssignMacroToFormControl-AssignMacroToFormControl.java" >}}

## Manipulate Document Properties in Excel

Aspose.Cells for Java API has exposed the WorkbookMetadata class that is lightweight as compared to Workbook class and allows loading the spreadsheet in order to manipulate the document properties in a simpler & more efficient way. In addition to the aforesaid class, the Aspose.Cells for Java 8.6.0 has also exposed the MetadataOptions class and MetadataType enumeration that can be used to specify the type of properties to be updated.

The following code snippet demonstrates how to use the newly exposed WorkbookMetadata & MetadataOptions classes to add a custom property to the spreadsheet while using Aspose.Cells for Java API.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-UsingWorkbookMetadata-UsingWorkbookMetadata.java" >}}

## Restrict the Generation of Frame Scripts for HTML Conversion

Aspose.Cells for Java 8.6.0 has exposed the HtmlSaveOptions.ExportFrameScriptsAndProperties property that can be used to [control the generation of scripts such as Frames & Document Properties while exporting the spreadsheets in HTML format][4]. The aforesaid boolean type property has the default value of true, that means; the resultant HTML will contain the scripts related to the frames as per standards of Excel application. Moreover, the resultant HTML code will contain the conditional comments that detects the browser type and adjusts the layout accordingly. Setting this property to false will direct the Aspose.Cells APIs not to generate frame scripts and conditional comments. In this case, the resultant HTML can be viewed in any browser but it cannot be imported back while using Aspose.Cells APIs.

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Exposed OoxmlSaveOptions.UpdateZoom property that can be used to update the PageSetup.Zoom if PageSetup.FitToPagesWide and/or PageSetup.FitToPagesTall properties have been used to control the Worksheet scaling.
*   Improved the HTML & PDF rendering engines for alignment, layout and shape rendering while handling ODS and other spreadsheet formats.
*   Improved the calculation engine to provide support for CORREL, RSQ, STEYX Excel functions.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Cells for Java API][5].
*   [Download Aspose.Cells for Java][6].
*   [Aspose.Cells for Java online documentation][7] – help documentation and API reference documents.
*   [Aspose.Cells Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Assign+Macro+Code+to+Form+Control
[4]: https://docs.aspose.com/display/cellsjava/Disable+exporting+frame+scripts+and+document+properties
[5]: http://products.aspose.com/cells/java
[6]: http://downloads.aspose.com/cells/java
[7]: http://docs.aspose.com/display/cellsjava/home
[8]: https://forum.aspose.com/
[9]: https://blog.aspose.com/
[10]: https://github.com/asposecells/Aspose_Cells_Java




