---
title: 'Render Excel Worksheet to Graphics2D Context using Java'
date: Mon, 24 Aug 2015 14:34:38 +0000
draft: false
url: /2015/08/24/render-excel-worksheet-to-graphics2d-context-using-java-excel-api/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of Aspose.Cells for Java 8.5.2. This month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.5.2][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Render Excel Worksheet to Graphics Context using Java

Aspose.Cells for Java APIs have exposed an overloaded version of SheetRender.toImage method that can accept an instance of java.awt.Graphics2D along with usual parameters to render the Worksheet in Graphics2D context. This feature is helpful in scenario where you wish to get high (scalable) print quality by redirecting the Graphics2D context to PostScript printer and create a PDF from the PostScript.

Following code snippet demonstrates how to use the newly exposed SheetRender.toImage method to [render the Worksheet in Graphics2D context][3].

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-RenderWorksheetToGraphicContext-ReleaseUnmanagedResources.java" >}}

## Access Cell by PivotField Name

Aspose.Cells for Java now provides the PivotTable.getCellByDisplayName method to [obtain the Cell reference by PivotField display name][4]. This method is useful in scenarios where the application requirement is to format the PivotField header in the PivotTable.

The following sample code explains the usage of PivotTable.getCellByDisplayName method to style the PivotField header.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-GetCellObject-GetCellObject.java" >}}

## Change Shape's Adjustment Values

Aspose.Cells for Java 8.5.2 has exposed the Geometry.getShapeAdjustValues method that can be used to [make changes to the adjustment points within the shapes][5]. Please note, Microsoft Excel application displays the adjustments points as yellow diamond nodes while allowing to change the arc for rounded rectangle, point location for a triangle, top width of a trapezoid, and shape of head & tail for arrows.

## ConsolidationFunction for the DataFields of PivotTable

Aspose.Cells APIs provide the means to [apply Consolidation Function to DataFields][6] (or value fields) of the PivotTable. In Microsoft Excel, you can right-click the value field and then select Value Field Settings... option and then select the tab Summarize Values By. From there, you can select any Consolidation Function of your choice like Sum, Count, Average, Max, Min, Product, Distinct Count etc.

Aspose.Cells provides ConsolidationFunction enumeration to support the following consolidation functions.

*   ConsolidationFunction.AVERAGE
*   ConsolidationFunction.COUNT
*   ConsolidationFunction.COUNT\_NUMS
*   ConsolidationFunction.DISTINCT\_COUNT
*   ConsolidationFunction.MAX
*   ConsolidationFunction.MIN
*   ConsolidationFunction.PRODUCT
*   ConsolidationFunction.STD\_DEV
*   ConsolidationFunction.STD\_DEVP
*   ConsolidationFunction.SUM
*   ConsolidationFunction.VAR
*   ConsolidationFunction.VARP

The following code applies Average consolidation function to first DataField and DistinctCount consolidation function to second DataField of a sample PivotTable.

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-PivotTables-ConsolidationFunctions-ConsolidationFunctions.java" >}}

## Other Enhancements & Improvements

The most notable  enhancements in this release are as follow:

*   Exposed SaveOptions.MergeAreas property to handle scenarios if a spreadsheet has too many individual cells with validation applied, there are chances that the resultant spreadsheet may get corrupted. One possible solution is to merge the cells with identical validation rules or you can now use the SaveOptions.MergeAreas property to direct the API to auto-merge the CellAreas before saving operation.
*   Improved the HTML & PDF rendering for alignment and layout.
*   Improved overall memory consumption.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Cells for Java API][7].
*   [Download Aspose.Cells for Java][8].
*   Aspose.Cells for Java online documentation – help documentation and API reference documents.
*   [Aspose.Cells Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Render+Worksheet+to+Graphic+Context
[4]: https://docs.aspose.com/display/cellsjava/Get+the+Cell+object+by+DisplayName+of+PivotField+of+PivotTable
[5]: https://docs.aspose.com/display/cellsjava/Change+Adjustment+Values+of+the+Shape
[6]: https://docs.aspose.com/display/cellsjava/Formatting+Pivot+Table#FormattingPivotTable-ApplyingConsolidationFunctiontoDataFieldsofPivotTable
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/
[11]: https://github.com/asposecells/Aspose_Cells_Java




