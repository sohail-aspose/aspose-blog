---
title: 'Set Margins of Comment or Shape and Specify Formula Fields while Importing Data to Worksheet using Aspose.Cells for Java 18.2'
date: Wed, 21 Feb 2018 05:51:16 +0000
draft: false
url: /2018/02/21/set-margins-of-comment-or-shape-and-specify-formula-fields-while-importing-data-to-worksheet-using-aspose.cells-for-java-18.2/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Set Shape and Comment Margins in Excel in Java', 'Specify Formula Fields in Data Import to Excel in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 18.2][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Set Margins of Comment or Shape inside the Worksheet

Aspose.Cells allows you to set the margins of any shape or comment using the **Shape.TextBody.TextAlignment** property. This property returns the object of **ShapeTextAlignment** class which has different properties e.g. TopMarginPt, LeftMarginPt, BottomMarginPt, RightMarginPt etc. that can be used to set the top, left, bottom and right margins. For more detail, please see the following article.

*   [Set Margins of Comment or Shape inside the Worksheet][4]

The following code loads the sample Excel file and accesses its shapes one by one and sets their top, left, bottom and right margins.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "DrawingObjects-SetMarginsOfCommentOrShapeInsideTheWorksheet.java" >}}

## Specify Formula Fields while Importing Data to Worksheet

You can specify formula fields when you import data into your worksheet using the **ImportTableOptions.setFormulas()** method. This method takes the Boolean array where the value true means the field is a formula field. For example, if the third field is a formula field, then third value in the array will be true. For more detail, please see the following article.

*   [Specify Formula Fields while Importing Data to Worksheet][5]

## Specify Maximum Rows of Shared Formula

Aspose.Cells provides the **Workbook.Settings.MaxRowsOfSharedFormula** property that can be used to specify the maximum rows of the shared formula. The shared formula will be split into several shared formulas if the total rows of the shared formula are greater than it. For more detail, please see the following article.

*   [Specify Maximum Rows of Shared Formula][6]

## Control External Resources using WorkbookSetting.StreamProvider

Sometimes, your Excel file contains external resources e.g. linked images, etc. Aspose.Cells allows you to control these external resources using **Workbook.Settings.StreamProvider** which takes the implementation of **IStreamProvider** interface. Whenever you will try to render your worksheet containing external resources e.g. linked images, the methods of IStreamProvider interface will be invoked which will enable you to take appropriate actions for your external resources. For more detail, please see the following article.

*   [Control External Resources using WorkbookSetting.StreamProvider][7]

## Filter Defined Names while loading Workbook

Aspose.Cells allows you to filter or remove defined names present inside the workbook. Please use **LoadDataFilterOptions.DEFINED\_NAMES** to load defined names and use **~LoadDataFilterOptions.DEFINED\_NAMES** to remove them while loading the workbook. Please note, if you will remove defined names, then formulas inside the workbook may break up. For more detail, please see the following article.

*   [Filter Defined Names while loading Workbook][8]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Download Aspose.Cells for Java from Maven][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.2/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.2+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Set+Margins+of+Comment+or+Shape+inside+the+Worksheet
[5]: https://docs.aspose.com/display/cellsjava/Specify+Formula+Fields+while+Importing+Data+to+Worksheet
[6]: https://docs.aspose.com/display/cellsjava/Specify+Maximum+Rows+of+Shared+Formula
[7]: https://docs.aspose.com/display/cellsjava/Control+External+Resources+using+WorkbookSetting.StreamProvider
[8]: https://docs.aspose.com/display/cellsjava/Filter+Defined+Names+while+loading+Workbook
[9]: https://products.aspose.com/cells/java
[10]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java




