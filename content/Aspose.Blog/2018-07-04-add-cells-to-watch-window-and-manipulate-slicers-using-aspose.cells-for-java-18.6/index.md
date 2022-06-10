---
title: 'Add Cells to Watch Window in Excel using Java'
date: Wed, 04 Jul 2018 13:45:59 +0000
draft: false
url: /2018/07/04/add-cells-to-watch-window-and-manipulate-slicers-using-aspose.cells-for-java-18.6/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Add cells to watch window in Excel in Java', 'Work with watch windows in Excel in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 18.6][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Add Cells to Watch Window in Excel using Java

Microsoft Excel Watch Window is a useful tool to watch the cell values and its formulas conveniently in a window. You can open the Watch Window using Microsoft Excel by clicking the **Formulas > Watch Window**. It has **Add Watch** button that can be used to add the cells for inspection. Similarly, you can use **Worksheet.getCellWatches().add()** method to add cells into Watch Window using Aspose.Cells API.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Formulas-AddCellsToMicrosoftExcelFormulaWatchWindow.java" >}}

Please see the following article for more detail on this topic.

*   [Add Cells to Microsoft Excel Formula Watch Window][3]

## Working with Slicers in Excel using Java

Slicers are used to filter data quickly. It provides buttons that user can click to filter Table or Pivot Table data. Whenever Slicer buttons are selected or deselected, it shows the current filtering state that helps the user to understand what precisely has been filtered in the Pivot Table. Please see the following articles that explain how to work with Slicers using Aspose API.

*   [Create Slicer to a Pivot Table][4]
*   [Formatting Slicer][5]
*   [Removing Slicer][6]
*   [Rendering Slicer][7]
*   [Updating Slicer][8]

The following sample code loads an Excel file that contains an existing Slicer. It unselects the 2nd and 3rd items of Slicer to refresh it. It then applies the formatting/style of the Slicer and finally describes how to remove the Slicer.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Slicers-UpdatingSlicer.java" >}}

## Add Custom XML Parts and Select Part by ID

Custom XML Parts are the XML data that is stored inside the Microsoft Excel documents and are used by the applications that deal with them. There is no direct way of adding them using Microsoft Excel UI at the moment. However, you can add them programmatically in various ways e.g. using VSTO, using Aspose.Cells etc. Please use **Workbook.getCustomXmlParts().add()** method if you want to add Custom XML Part using Aspose.Cells API. You can also set its ID, using the **CustomXmlPart.ID** property. Similarly, if you want to select Custom XML Part by ID, you can use **Workbook.getCustomXmlParts().selectByID()** method.

*   [Add Custom XML Parts and Select them by ID][9]

## Get Address, CellCount Offset, EntireColumn and EntireRow of the Range

Aspose.Cells has added few new utility methods inside the Range object that help the user finding Address, Cell Count, Offset, Entire Column and Entire Row of the Range object. Please see the following article for more detail on this.

*   [Get Address, Cell Count, Offset, Entire Column and Entire Row of the Range][10]

## Extract Text from the Gear Type SmartArt Shape

Aspose.Cells can extract text from the Gear Type Smart Art Shape. In order to do so, you should first convert the Smart Art Shape to Group Shape using the **Shape.getResultOfSmartArt()** method. Then you should get the array of all the Individual Shapes forming the Group Shape using the **GroupShape.getGroupedShapes()** method. Finally, you can iterate all of the Individual Shapes one by one in a loop and extract their text using the **Shape.getText()** method.

*   [Extract Text from the Gear Type SmartArt Shape][11]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][12].
*   [Download Aspose.Cells for Java][13].
*   [Aspose.Cells for Java Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.6/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.6+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Add+Cells+to+Microsoft+Excel+Formula+Watch+Window
[4]: https://docs.aspose.com/display/cellsjava/Create+Slicer+to+a+Pivot+Table
[5]: https://docs.aspose.com/display/cellsjava/Formatting+Slicer
[6]: https://docs.aspose.com/display/cellsjava/Removing+Slicer
[7]: https://docs.aspose.com/display/cellsjava/Rendering+Slicer
[8]: https://docs.aspose.com/display/cellsjava/Updating+Slicer
[9]: https://docs.aspose.com/display/cellsjava/Add+Custom+XML+Parts+and+Select+them+by+ID
[10]: https://docs.aspose.com/display/cellsjava/Get+Address+Cell+Count+Offset+Entire+Column+and+Entire+Row+of+the+Range
[11]: https://docs.aspose.com/display/cellsjava/Extract+Text+from+the+Gear+Type+SmartArt+Shape
[12]: https://products.aspose.com/cells/java
[13]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[14]: https://docs.aspose.com/display/cellsjava/home
[15]: https://apireference.aspose.com/java/cells
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-Java




