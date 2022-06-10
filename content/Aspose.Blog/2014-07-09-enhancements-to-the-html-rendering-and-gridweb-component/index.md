---
title: 'Enhancements to the HTML Rendering and GridWeb Component with Aspose.Cells for Java 8.1.1'
date: Wed, 09 Jul 2014 08:02:14 +0000
draft: false
url: /2014/07/09/enhancements-to-the-html-rendering-and-gridweb-component/
author: Babar Raza
summary: ''
tags: ['API', 'API to Create Spreadsheets', 'API to Manipulate Spreadsheets', 'Aspose.Cells', 'Babar Raza', 'Formula Engine', 'GridWeb for Java', 'HTML Rendering', 'Worksheet Scenarios']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the monthly release of [Aspose.Cells for Java][1], version 8.1.1. Our team has been hard at work bringing many useful improvements to this edition of the Aspose.Cells API. You can start exploring the newly added features & enhancements immediately, but before you head to the [download section][2], here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above. If you are going to upgrade the API, please refer to the article Public API Changes in Reference to 8.1.1 of Aspose.Cells for Java.

## Enhancements to HtmlSaveOptions

The class HtmlSaveOptions has been enhanced to render HTML results with better layout. The feature is now available through the Boolean type PresentationPreference property which can be set to true while exporting spreadsheets to HTML format to get a better presentation layout. For further elaboration on the topic, please check the detailed article on using the PresentationPreference option.

## Enhancements to the CellsException

With previous releases of Aspose.Cells for Java API, when a possibly damaged spreadsheet was loaded in an instance of Workbook, the API tended to throw a generic message not mentioning where the problem could be. We have changed this behavior since 8.1.1, so that now the API throws an exception with a meaningful message to point out where (which cell) and what (formula expression) causes the exception when reading the template file.

## Support for Scenarios

Scenarios are part of a suite of commands called what-if analysis tools provided by Microsoft Excel. What-if analysis is the process of changing the values in cells to see how those changes affect the outcome of formulas on the worksheet. They are useful for forecasting and financial models. Microsoft Excel saves a set of values in a scenario, and can automatically substitute these values in the worksheet.

With this release of Aspose.Cells for Java, Aspose has provided support for scenarios to allow developers to create, manipulate and remove scenarios without needing Microsoft Excel. Aspose.Cells for Java has exposed many useful classes to make this task possible. A few of the most important classes are listed below. A detailed article is available at working with scenarios.

*   Scenario: Represents an individual scenario.
*   ScenarioCollection: Represents a collection of scenarios.
*   ScenarioInputCellCollection: Represents a list of input cells for a particular scenario.
*   ScenarioInputCell: Represents an input cell from the collection of input cells for a particular scenario.

## Support for GridWeb Component

Aspose.Cells for Java 8.1.1 has been packaged with the GridWeb component that can be used in Java based web applications to render and visually manipulate spreadsheets on the go. The download package also contains a demo - gridwebdemo.war - that you can deploy on your web server to see the component in action. Please check the detailed article on how to run Aspose.Cells for GridWeb Java demos in Apache Tomcat Server. The demo application can be downloaded from [here][3].

## Bug Fixes

We have addressed several important problems with this release. A few of the most notable issues are listed below.

*   Conditional formatting rendered incorrectly in PDF.
*   Fonts related issues while rendering spreadsheets as PDF.
*   Transparency problem with PNG.
*   Localized formula formats.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Cells support forum][4] for a chat.




[1]: https://products.aspose.com/cells/java
[2]: https://downloads.aspose.com/cells/java
[3]: https://downloads.aspose.com/cells/java
[4]: https://forum.aspose.com/




