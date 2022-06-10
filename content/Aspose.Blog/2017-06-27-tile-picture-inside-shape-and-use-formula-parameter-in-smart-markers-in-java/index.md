---
title: 'Tile Picture inside Shape and Use Formula parameter in Smart Markers in Java'
date: Tue, 27 Jun 2017 10:51:27 +0000
draft: false
url: /2017/06/27/tile-picture-inside-shape-and-use-formula-parameter-in-smart-markers-in-java/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](https://www.aspose.com/products/cells/java "Aspose.Cells for Java - Excel Java APIs")Aspose team is pleased to announce the release of [Aspose.Cells for Java 17.6][2]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][3]. Please check the [release notes][4] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Tile Picture as a Texture inside the Shape

Aspose.Cells supports image tiling feature which allows you to display images that are too large to be displayed entirely as a single unit on a typical computer. The feature allows you to display by segmenting it into smaller, more manageable image tiles.

```
//Load sample Excel file
Workbook wb = new Workbook("e:\\test2\\Book1.xlsx");

//Access first worksheet
Worksheet ws = wb.getWorksheets().get(0);
  
//Access first shape inside the worksheet
Shape sh = ws.getShapes().get(0);
  
//Tile Picture as a Texture inside the Shape 
sh.getFill().getTextureFill().setTiling(true);

//Save the output Excel file
wb.save("e:\\test2\\out1.xlsx"); 
```

Please see this article that explains how to Tile Picture as a Texture inside the Shape.

*   [Tile Picture as a Texture inside the Shape][5]

## Using Formula parameter in Smart Marker field

Sometimes, you need to embed formula in [Smart Markers][6]. Aspose.Cells allows you to make use of Formula parameter in Smart marker field. For more detail, please see this article.

*   [Using Formula parameter in Smart Marker field][7]

## Using OnAjaxCallFinishedClientFunction of GridWeb

_OnAjaxCallFinishedClientFunction_ is a client side function which is called when user copies some data into Aspose.Cells.GridWeb worksheet. This function is helpful when bulk of cells are updated and you want to keep track of those updated cells at client side (i.e., in web browsers like FireFox, Google Chrome etc.). See the following document/article for your reference.

*   [Using OnAjaxCallFinishedClientFunction of Aspose.Cells.GridWeb][8]

## Other Enhancements and Fixes

Aspose.Cells 17.6 has enhanced its core for more stability as well as fixed many critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Remove unnecessary older Web.config settings of Aspose.Cells.GridWeb like force script\_path and forcepath.
*   Group Rows in the worksheet - Aspose.Cells.GridWeb (JAVA).
*   Handled an exception, "The row index should not be inside the pivottable report" when rendering to HTML file format.
*   Handled an Exception, "java.lang.NullPointerException" when opening an ODS file via Aspose.Cells APIs.
*   Handled NullPointerException on creating Workbook instance from source Excel file.

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats, rendering shapes and drawing objects, rendering and manipulating charts, rendering HTML to Excel and vice versa, [rendering images from Excel worksheets][9],[rendering images files from charts][10]and[exporting Excel workbooks to PDF format][11]have been resolved. The formula calculation engine is further enhanced in the new release.

## Changes to the Public API

This version of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   Added _GridWeb.OnAjaxCallFinishedClientFunction_ property that lets you get or set the client side function name to be called when ajaxcall is finished.
*   Added enum _StyleModifyFlag.RelativeIndent_ attribute that represents relative indent.
*   Added _TextureFill.setTiling_ property that indicates whether tile picture as texture.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][12].
*   [Aspose.Cells for Java Download Section][13].
*   [Aspose.Cells for Java Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][17] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][18] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java"
[2]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.6/ "Download Aspose.Cells for Java 17.6"
[3]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[4]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.6+Release+Notes "Release Notes of Aspose.Cells for Java 17.6"
[5]: https://docs.aspose.com/display/cellsjava/Tile+Picture+as+a+Texture+inside+the+Shape
[6]: https://docs.aspose.com/display/cellsjava/Using+Smart+Markers
[7]: https://docs.aspose.com/display/cellsjava/Using+Formula+parameter+in+Smart+Marker+field
[8]: https://docs.aspose.com/display/cellsjava/Using+OnAjaxCallFinishedClientFunction+of+GridWeb
[9]: https://docs.aspose.com/display/cellsjava/Converting+Worksheet+to+Different+Formats
[10]: https://docs.aspose.com/display/cellsjava/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsjava/Converting+Workbook+to+Different+Formats#ConvertingWorkbooktoDifferentFormats-ConvertingExceltoPDF
[12]: https://www.aspose.com/products/cells/java
[13]: https://downloads.aspose.com/cells/java
[14]: https://docs.aspose.com/display/cellsjava/home
[15]: https://apireference.aspose.com/java/cells
[16]: https://forum.aspose.com/c/cells
[17]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[18]: https://github.com/asposecells/Aspose_Cells_Java




