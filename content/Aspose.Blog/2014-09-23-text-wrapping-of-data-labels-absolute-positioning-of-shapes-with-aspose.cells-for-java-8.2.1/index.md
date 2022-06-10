---
title: 'Text Wrapping of Data Labels &amp; Absolute Positioning of Shapes with Aspose.Cells for Java 8.2.1'
date: Tue, 23 Sep 2014 15:09:45 +0000
draft: false
url: /2014/09/23/text-wrapping-of-data-labels-absolute-positioning-of-shapes-with-aspose.cells-for-java-8.2.1/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Chart Data Labels', 'Chart2Image', 'Excel 2013', 'Excel API', 'Spreadsheet Creation', 'Spreadsheet Manipulation', 'text wrapping']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of Aspose.Cells for Java 8.2.1. Our team has been hard at work bringing many useful improvements to the latest edition of Aspose.Cells library. You can explore the new features & enhancements immediately. Before you head to the download section, here is a look at the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the [release notes for Aspose.Cells for Java 8.2.1][1].

## Text Wrapping for Chart Data Labels

Microsoft Excel 2013 allows users to wrap or unwrap data label text in a chart. The default is the wrapped state. Aspose.Cells provides the setTextWrapped method for the DataLabels class, which can be set to true or false in order to [enable or disable the data label text wrapping feature][2]. Moreover, you can use the isTextWrapped method to find out if a data label's text is already wrapped.

## Find Absolute Position of Shape in a Worksheet

Before the release of Aspose.Cells for Java 8.2.1, finding the absolute position of a shape in the worksheet required a lot of mathematical calculation. Even after writing dozens lines of source code developers had to use the "hit & try" mechanism to find out the exact position of a shape. With the release of Aspose.Cells for Java 8.2.1, you can simply call the Shape.getLeftToCorner and Shape.getTopToCorner methods to [get the absolute position in the unit of pixels for a shape][3].

## Cell Data Validation

Aspose.Cells for .NET is an easy to use spreadsheet creation, manipulation and conversion API that provides all the features that Microsoft Excel provides. Cell validation is one of the features that spreadsheet designers widely use to stop users from inserting invalid values into a cell. With the release of Aspose.Cells for Java 8.2.1, the API has exposed a simple means to [identify if data validation has been applied on a particular cell][4]. You can use the Cell.getValidation method to acquire applied validation. Moreover, you can use the Validations.getValidationInCell method to acquire the validation applied on any cell by providing its row and column indices.

In addition to the feature discussed above, you can verify if a given value satisfies the data validation rules for a cell. This feature is useful when you want to [verify if the value entered into a cell satisfies the data validation rule on the fly][5]. Aspose.Cells API has exposed the getValidationValue method for Cell class. If the value in a cell does not satisfy the data validation rules, the Cell.getValidationValue method returns false.

## Other Enhancements & Improvements

Aspose.Cells for Java 8.2.1 sees the base code tweaked and the core functionality closer to Aspose.Cells for .NET 8.2.1, from which Aspose.Cells for Java is ported. The latest release has fixed numerous problems, and the most notable of these  enhancements are:

*   Enhanced the PDF rendering engine to handle shapes more appropriately.
*   Tweaked the HTML rendering engine for better layout.
*   Improved Chart2Image feature to handle text boxes present in charts.

Please visit the [documentation][6] for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][7].




[1]: https://downloads.aspose.com/cells/java
[2]: http://docs.aspose.com/display/cellsjava/Disable+Text+Wrapping+for+Data+Labels+of+the+Chart
[3]: http://docs.aspose.com/display/cellsjava/Finding+Absolute+Position+of+Shape+inside+the+Worksheet
[4]: http://docs.aspose.com/display/cellsjava/Get+Validation+applied+on+a+Cell
[5]: http://docs.aspose.com/display/cellsjava/Verify+that+Cell+Value+satisfies+Data+Validation+Rules
[6]: http://docs.aspose.com/display/cellsjava/Home
[7]: http://forum.aspose.com




