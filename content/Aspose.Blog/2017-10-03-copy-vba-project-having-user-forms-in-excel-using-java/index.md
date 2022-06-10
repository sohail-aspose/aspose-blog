---
title: 'Copy VBA Project having User Forms in Excel using Java'
date: Tue, 03 Oct 2017 13:09:08 +0000
draft: false
url: /2017/10/03/copy-vba-project-having-user-forms-in-excel-using-java/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 17.9][1]. This release includes some of valuable features and enhancements along with critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Copy VBA Project having User Form from Template to Target Workbook

Aspose.Cells allows you to copy VBA project from one Excel file into another Excel file. VBA project consists of various types of modules i.e. Document, Procedural, Designer etc. All modules can be copied with simple code but for Designer module, there is some extra data called Designer Storage needs to be accessed or copied. The following two methods deal with Designer Storage.

*   **VbaModuleCollection.getDesignerStorage()**
*   **VbaModuleCollection.addDesignerStorage()**

Please see the following article for more detail and sample code.

*   [Copy VBA Macro UserForm DesignerStorage from Template to Target Workbook  
    ](https://docs.aspose.com/display/cellsjava/Copy+VBA+Macro+UserForm+DesignerStorage+from+Template+to+Target+Workbook)

## Send Shape Front or Back inside the Worksheet

When there are multiple shapes present in the same location then how will they be visible is decided by their z-order positions. Aspose.Cells provides **Shape.toFrontOrBack()** method which changes the z-order position of the shape. If you want to send shape to back you will use negative number like -1, -2, -3 etc. and if you want to send shape to front, you will use positive number like 1, 2, 3 etc.

*   [Send Shape Front or Back inside the Worksheet][4]

This screenshot shows the effect of the code in the above article on the source workbook. As you can see, the z-order positions of shapes have been changed as per sample code.



{{< figure align=center src="images/Send-Shape-Front-or-Back-inside-the-Worksheet-300x221.png" alt="">}}


## GridWeb displays Comment as Tooltip like Microsoft Excel

GridWeb provides the feature to [add, remove or get comments inside the worksheet][5]. However, now it also displays comments as Tooltip like Microsoft Excel displays as shown in this screenshot.



{{< figure align=center src="images/GridWeb-displays-comment-as-Excel-Tooltip-300x207.png" alt="">}}


## Sort Data in Column with Custom Sort List

You can sort data in the column using custom list. This can be done using **DataSorter.addKey(int key, SortOrder order, String customList)** method. However, this method works only if the items in custom list do not have commas inside them. If they have commas like **"USA,US", "China,CN"** etc., then you must use **DataSorter.addKey(int key, SortOrder order, String\[\] customList)** method. Here, the last parameter is not String but Array of Strings.

*   [Sort Data in Column with Custom Sort List][6]

```
//Load the source Excel file
Workbook wb = new Workbook(dirPath + "sampleSortData_CustomSortList.xlsx");
  
//Access first worksheet
Worksheet ws = wb.getWorksheets().get(0);
  
//Specify cell area - sort from A1 to A40
CellArea ca = CellArea.createCellArea("A1", "A40");
  
//Create Custom Sort list
String[] customSortList = new String[] { "USA,US", "Brazil,BR", "China,CN", "Russia,RU", "Canada,CA" };
  
//Add Key for Column A, Sort it in Ascending Order with Custom Sort List
wb.getDataSorter().addKey(0, SortOrder.ASCENDING, customSortList);
wb.getDataSorter().sort(ws.getCells(), ca);
  
//Save the output Excel file
wb.save(dirPath + "outputSortData_CustomSortList.xlsx"); 
```

## Add PDF Bookmarks with Named Destinations

Named Destinations are special kinds of bookmarks or links in PDF that do not depend on PDF pages. It means, if pages are added or deleted from PDF, bookmarks may become invalid but named destinations will remain intact. To create Named Destination, please use the **PdfBookmarkEntry.setDestinationName()** method.

*   [Add PDF Bookmarks with Named Destinations][7]

## Control loading of External Resources in MS Excel Workbook while rendering to PDF

Your Excel file may contain external resources e.g. linked images or objects. When you convert your Excel file to Pdf, Aspose.Cells retrieves these external resources and renders them to Pdf. But sometimes, you do not want to load these external resources and more than that, you want to manipulate them. You can do this using **PdfSaveOptions.StreamProvider** which implements the **IStreamProvider** interface.

*   [Control loading of External Resources in MS Excel Workbook while rendering to PDF][8]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Aspose.Cells for Java Download Section][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.9/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.9+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Send+Shape+Front+or+Back+inside+the+Worksheet
[5]: https://docs.aspose.com/display/cellsjava/Create+Remove+and+Get+GridCell+Comments
[6]: https://docs.aspose.com/display/cellsjava/Sort+Data+in+Column+with+Custom+Sort+List
[7]: https://docs.aspose.com/display/cellsjava/Add+PDF+Bookmarks+with+Named+Destinations
[8]: https://docs.aspose.com/display/cellsjava/Control+loading+of+External+Resources+in+MS+Excel+Workbook+while+rendering+to+PDF
[9]: https://www.aspose.com/products/cells/java
[10]: https://downloads.aspose.com/cells/java
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java




