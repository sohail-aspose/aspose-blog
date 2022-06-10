---
title: 'Export Hidden Worksheets to HTML using Java'
date: Wed, 11 Jun 2014 10:04:57 +0000
draft: false
url: /2014/06/11/restrict-the-api-to-use-only-one-font-location-export-hidden-worksheets-to-html-and-more-in-aspose.cells-for-java-8.1.0/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells for Java', 'Babar Raza', 'Export Spreadsheets to PDF', 'JVM Arguments', 'Linux Distributions', 'Required TTF', 'Required TrueType Fonts. Aspose.Cells TrueType Fonts', 'Saving Spreadsheets as PDF', 'Saving Spreadsheets to Images', 'XPS']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the monthly release of [Aspose.Cells for Java][1] 8.1.0. Our team has been hard at work bringing many useful improvements with the latest edition of Aspose.Cells library. You can immediately start exploring the newly added features & enhancements. Before you head to the [download section][2], here is a look at just a few of the biggest features in this month’s release.

For a full list of bug fixes and improvements please refer to the release notes in the above link.

## Restrict the API to Use Only One Font Location

This newly added feature allows developers to restrict the API to use only one font location while rendering spreadsheets. Users may now set the JVM arguments to tell the API where to look for the required fonts or use the System.setProperty method in application code to achieve the same. More details on this topic can be found on the [Specifying TrueType Fonts Location][3]. Please also check [How Aspose.Cells uses the TrueType font behind the scene][4].

## Enhancements to the HtmlSaveOptions Class

Aspose.Cells for Java API now provides get/set methods for the ExportHiddenWorksheet property exposed by the HtmlSaveOptions class. The aforesaid Boolean property allows the users to choose whether to render the hidden worksheets or not. The default value is true, meaning the hidden worksheet will be rendered as HTML; switching to false excludes hidden worksheets from the rendering process. More details on this topic can be found on the Prevent Exporting Hidden Worksheet Contents while Saving to HTML.

## Enhancements to the PivotTable Class

Aspose.Cells has been trying to provide all features that Microsoft Excel offers. One step further, Aspose.Cells has exposed the getter/setters for the DisplayNullString & NullString properties for PivotTable class to handle the Pivot Table option “For empty cells show” offered by the Microsoft Excel. These properties allow the users to set display option for the empty cells inside the Pivot Table to any specified string.

## Bug Fixes

Aspose.Cells for Java 8.1.0 has provided fix for several important issues, such as a couple of problems related to rendering spreadsheets as PDF on Linux platform, exporting spreadsheets to HTML, print quality & page setup.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Cells support forum][5] for a chat.




[1]: https://products.aspose.com/cells/java
[2]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry551145.aspx
[3]: https://docs.aspose.com/cells/java/how-to-specify-truetype-fonts-location/
[4]: https://docs.aspose.com/cells/java/how-aspose-cells-uses-truetype-fonts/
[5]: https://forum.aspose.com/




