---
title: 'Control the Conversion of Large Numeric Value to Exponential Notation in Excel using Java'
date: Fri, 29 Apr 2016 14:12:53 +0000
draft: false
url: /2016/04/29/control-the-conversion-of-large-numeric-value-to-exponential-notation-in-excel-using-java/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java][1] 8.8.0. This month’s release includes new features, enhancements, and bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Control the Conversion of Large Numeric Value to Exponential Notation

As per default behavior, if a numeric value is larger than the threshold, the API converts such values to exponential notation while importing HTML segment/files to Aspose.Cells object model. In the past, we could use the HTMLLoadOptions.ConvertNumericData property to control the conversion of textual values to numeric data, however, this approach has its own drawbacks. For instance, if there are more than one column containing the numeric values, setting the HTMLLoadOptions.ConvertNumericData property to false will direct the Aspose.Cells APIs to keep all values in textual format. In such case, all formatting from the numeric values will be lost.

In order to handle the situations where users wish to retain the format of all numeric values as well as keep the data in its original state, the Aspose.Cells for Java 8.8.0 has exposed the HTMLLoadOptions.KeepPrecision property. The Boolean type property allows controlling the conversion of large numeric values to exponential notation. When set to true, the numeric values larger than 15 digits will be imported as it is.

Here is the simple usage scenario demonstrating the usage of HTMLLoadOptions.KeepPrecision property to avoid the conversion of large numbers to exponential notation while importing data from Html.



## Delete Redundant Spaces from HTML

Aspose.Cells for Java 8.8.0 has exposed the HTMLLoadOptions.DeleteRedundantSpaces property to control the preservation of redundant spaces after the line break tag (<BR> tag) in HTML. If the aforementioned property is set to true the API will delete all the redundant spaces while importing the HTML in Aspose.Cells object mode. The HTMLLoadOptions.DeleteRedundantSpaces property has the default value as false, that means, all the redundant spaces are preserved in the resultant spreadsheet.

## Detect if Cell Value Starts with Single Quote

Aspose.Cells for Java 8.8.0 has exposed the Style.QuotePrefix property to detect if the cell value starts with single quote mark. With previous revisions of Aspose.Cells APIs, it was not possible to distinguish between the text values such as sample and 'sample.

Here is the simple usage scenario of Style.QuotePrefix property to [find if the cell value starts with single quote mark][4].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Articles-DetectCellValueStartsWithSingleQuote.java" >}}

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Ability to [use image markers while grouping data in smart markers][5].
*   Ability to [find Query Tables and List Objects related to external data connections][6].
*   The improved PDF rendering engine for chart objects.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][7].
*   [Aspose.Cells for Java Download Section][8].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Java API Reference Guide][9] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][10] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][11] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][12] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: http://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+8.8.0+Release+Notes
[3]: http://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: https://docs.aspose.com/display/cellsjava/Find+if+the+cell+value+starts+with+single+quote+mark
[5]: http://docs.aspose.com/display/cellsjava/Using+Image+Markers+while+Grouping+Data+in+Smart+Markers
[6]: https://docs.aspose.com/display/cellsjava/Find+Query+Tables+and+List+Objects+related+to+External+Data+Connections
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/
[12]: https://github.com/asposecells/Aspose_Cells_Java




