---
title: 'Tile Picture inside Shape within Excel Spreadsheets using Java'
date: Mon, 26 Jun 2017 18:24:50 +0000
draft: false
url: /2017/06/26/tile-picture-inside-shape-and-use-formula-parameter-in-smart-markers-in-.net/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.6][1]. This release includes a few new features and other enhancements along with some critical bug fixes that further improve the overall stability of the APIs. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Tile Picture as a Texture inside the Shape using C#

Aspose.Cells supports image tiling feature which allows you to display images that are too large to be displayed entirely as a single unit on a typical computer. The feature allows you to display by segmenting it into smaller, more manageable image tiles.

```
//Load sample Excel file
Workbook wb = new Workbook("e:\\test2\\Book1.xlsx");

//Access first worksheet
Worksheet ws = wb.Worksheets[0];

//Access first shape inside the worksheet
Shape sh = ws.Shapes[0];

//Tile Picture as a Texture inside the Shape 
sh.Fill.TextureFill.IsTiling = true;

//Save the output Excel file
wb.Save("e:\\test2\\out1.xlsx");
```

Please see this article that explains how to Tile Picture as a Texture inside the Shape.

*   [Tile Picture as a Texture inside the Shape][4]

## Using Formula Parameter in Smart Marker Field

Sometimes, you need to embed formula in [Smart Markers][5]. Aspose.Cells allows you to make use of Formula parameter in Smart marker field. For more detail, please see this article.

*   [Using Formula parameter in Smart Marker field][6]

## Using OnAjaxCallFinishedClientFunction of GridWeb

_OnAjaxCallFinishedClientFunction_ is a client side function which is called when user copies some data into Aspose.Cells.GridWeb worksheet. This function is helpful when bulk of cells are updated and you want to keep track of those updated cells at client side (i.e., in web browsers like FireFox, Google Chrome etc.). See the following document/article for your reference.

*   [Using OnAjaxCallFinishedClientFunction of Aspose.Cells.GridWeb][7]

## Other Enhancements and Fixes

Aspose.Cells 17.6 has enhanced its core for more stability as well as fixed many critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Enquote all attribute values in HTML.
*   Support some new functions of Office 365.
*   Remove unnecessary older Web.config settings of Aspose.Cells.GridWeb like force script\_path and forcepath.
*   [Group Rows and Create Subtotal - Aspose.Cells.GridWeb][8].
*   Handled an exception, "Input string was not in a correct format" when loading an XLSX file format.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   Added _GridWeb.OnAjaxCallFinishedClientFunction_ property that lets you get or set the client side function name to be called when ajaxcall is finished.
*   Added enum _StyleModifyFlag.RelativeIndent_ attribute that represents relative indent.
*   Added _TextureFill.IsTiling_ property that indicates whether tile picture as texture.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][9].
*   [Aspose.Cells for .NET Download Section][10].
*   [Aspose.Cells for .NET Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.6/
[2]: https://docs.aspose.com/cells/net/aspose-cells-for-net-17-6-release-notes/
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/cells/net/tile-picture-as-a-texture-inside-the-shape/
[5]: https://docs.aspose.com/cells/net/using-smart-markers/
[6]: https://docs.aspose.com/cells/net/using-formula-parameter-in-smart-marker-field/
[7]: https://docs.aspose.com/cells/net/using-onajaxcallfinishedclientfunction-of-gridweb/
[8]: https://docs.aspose.com/cells/net/group-rows-and-create-subtotal/
[9]: https://products.aspose.com/cells/net
[10]: https://downloads.aspose.com/cells/net
[11]: https://docs.aspose.com/cells/net
[12]: https://apireference.aspose.com/
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




