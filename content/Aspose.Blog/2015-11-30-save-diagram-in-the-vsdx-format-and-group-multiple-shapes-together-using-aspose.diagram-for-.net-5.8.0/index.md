---
title: 'Save Visio Diagram in the VSDX Format and Group Multiple Shapes using C#'
date: Mon, 30 Nov 2015 13:37:05 +0000
draft: false
url: /2015/11/30/save-diagram-in-the-vsdx-format-and-group-multiple-shapes-together-using-aspose.diagram-for-.net-5.8.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the new version 5.8.0 of the [Aspose.Diagram for .NET][1] API. It includes the long awaited features of saving Visio diagrams in the latest VSDX format and grouping multiple shapes together to move all at once. Since from this version, developers would be able to read and write VSDX file formats. They would also be able to transform multiple shapes into one group shape.

Besides this, we have added support of saving Visio diagrams in the HTML format without the toolbar too. Many other defect fixes have been included, those consolidate overall diagram's elements, formatting like styles, borders, accuracy in positioning shapes and preserve properties and layers.

## Save Visio Diagram in the VSDX Format using C#

Aspose.Diagram API allows to save Visio diagrams in the VSDX format. The new VSDX format uses XML content and essentially saves drawing in a zipped compression that results in much smaller file sizes. To accomplish this task using Aspose.Diagram API, there is a new addition of the VSDX format in the SaveFileFormat enum. All the supported file formats are documented there: Product Overview

## Grouping Visio Shapes Together using C#

To work faster, developers can now group Visio shapes together using Aspose.Diagram API. They can do anything to a group of shapes like a single shape. The group shape can be resized, rotated and aligned with other shapes, and so on. Please refer to the following example topic: Grouping Shapes Together in the Visio Drawing

This release also covers many aspects in the export, layout, structure, performance and quality areas. Please check a list of fixed defects:

*   Fixed: Incorrect font when placing a shape from a VSX stencil.
*   Fixed: Characters of the shape's text items are mingling with each other.
*   Fixed: VSD to PDF conversion, the text items of the shapes are misplaced.
*   Fixed: VSD to PDF conversion, shapes text items at the top right corners are misplaced.
*   Fixed: VSD to PDF conversion, the text lines between the bullets are not aligned properly.
*   Fixed: VSD to PDF conversion, the table item is not preserved.
*   Fixed: Timeline start and finish dates are not taking effect.
*   Fixed: VSD to PDF / HTML conversion, an extra text item is added at left bottom.
*   Fixed: Shape id is greater than 32 bit.
*   Fixed: Incorrect Visio page properties.
*   Fixed: DiagramSaveOptions.AutoFitPageToDrawingContent property works partially.
*   Fixed: Layers disappear when setting AutoFitPageToDrawingContent save option.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new SaveToolBar option has been added in the HTMLSaveOptions class.
*   The VSDX format option has been added in the SaveFileFormat enum.
*   The Group method has been added in the ShapeCollection class.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][2].
*   [Download Aspose.Diagram for .NET][3]
*   [Aspose.Diagram for .NET docs][4] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/net
[2]: https://products.aspose.com/diagram
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[4]: https://docs.aspose.com/diagram/net
[5]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_diagram_NET




