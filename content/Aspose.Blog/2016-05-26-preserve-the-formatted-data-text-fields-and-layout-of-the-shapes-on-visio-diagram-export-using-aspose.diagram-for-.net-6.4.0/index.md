---
title: 'Preserve the Formatted Data, Text Fields and Layout of the Shapes on Visio Diagram Export using Aspose.Diagram for .NET 6.4.0'
date: Thu, 26 May 2016 15:58:13 +0000
draft: false
url: /2016/05/26/preserve-the-formatted-data-text-fields-and-layout-of-the-shapes-on-visio-diagram-export-using-aspose.diagram-for-.net-6.4.0/
author: Imran Rafique
summary: ''
tags: ['Convert Visio', 'Create a VSDX', 'Shape formatting', 'export Visio diagram', 'shape border', 'shape colors', 'shape font', 'shape text alignment', 'spacing between the shapes']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce that the new version 6.4.0 of Aspose.Diagram for .NET API is now live. This new version primarily improves converting Visio diagram to other supported file formats. It preserves the formatted data, text items, alignments, proper spacing between the shapes and overall structural layout of the diagram. This version also covers fixes of reported errors and various other enhancements.

## Render Multiple Colors in the Group Shape

Using Aspose.Diagram API, developers can create their own custom group shape from several non-group shapes. They might need a shape of the system that is not in one of the standard templates, and then fill colors in each sub shape to display various sections of the system. Similarly, one of our clients was trying to convert a Visio diagram made up of multiple traffic light shapes, but the traffic light colors were not being preserved in the resulting file. To accommodate this aspect, we have enhanced the API for rendering colors in Visio shapes.

## Border Style of the Shape

Using Aspose.Diagram API, developers can change the color, weight, or style of the outside border of a shape, or remove the border altogether. Visio diagrams can hold much more information than just graphics, so it is crucial for diagram export to preserve the same border style, arrows, connector line format and so on. This version has enhanced preserving border styles of the shapes on exporting the Visio diagram.

## Alignment and Absolute Positioning of the Shapes

Our clients export diagrams from Visio into another format for sharing with other stakeholders. The ability to export a Visio diagram provides developers a fast and easy programmatic way, consistent with the Microsoft Office Visio application. The export feature demands accuracy in alignment and absolute positioning of the shapes. We're continuously improving it in the each version and ensuring that all improvement activities are implemented and followed successfully.

This version also covers the issues of missing textual items of the shapes, partial rendering of the text, alignment of the shape text, wrong position of the shape and error messages while creating an empty VSDX or converting an existing VSDX to PDF. These bug fixes also improve the performance of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSD to PDF export - the color of circles inside the traffic signal boxes is not preserved.
*   Fixed: VSD to PDF export - Dashed lines are converted to solid lines.
*   Fixed: Misplaced text or incorrect line breaks when converting VSD to PDF format.
*   Fixed: VSD to PDF conversion, Shape's text with incorrect wrapping/layout.
*   Fixed: VSD to PDF conversion, incorrect layout of the text in shapes.
*   Fixed: VSD to SVG conversion, missing sub shapes or incorrect positions.
*   Fixed: VSD to SVG conversion, text items are misplaced.
*   Fixed: VSDX to SVG conversion, text items are misplaced.
*   Fixed: VDW to PDF conversion, the text items are messed up.
*   Fixed: VSD to PDF conversion, the text shape is misplaced.
*   Fixed: VSD to PDF conversion, the text items are not preserved.
*   Fixed: VSDX to PDF conversion, the embedded word document icon is missing.
*   Fixed: VSD to PDF conversion, table items are not preserved.
*   Fixed: VSD to PDF export, the dash type horizontal line turns into the solid line.
*   Fixed: VSDX to PDF export, the circular shapes of type metafile are missing.
*   Fixed: VSD to PDF export renders incorrect formatting of the bullets.
*   Fixed: VSD to HTML export renders incorrect formatting of the bullets.
*   Fixed: VSD to PDF export renders incorrect formatting of the bullets.
*   Fixed: VSD to HTML export renders incorrect formatting of the bullets.
*   Fixed: VSD to HTML export renders incorrect formatting of the bullets.
*   Fixed: VSD to PDF export aligns the shape's text incorrectly.
*   Fixed: VSD to HTML export aligns the shape's text incorrectly.
*   Fixed: VSD to PDF export - the word "STOP" is lost.
*   Fixed: VSD to PDF export - the "N" character in the North Arrow is lost.
*   Fixed: Open and save routine of a VSDX diagram has lost theme of the shapes.
*   Fixed: Open and save routine of a VSDX diagram has lost the arrows of connectors.
*   Fixed: Open and save routine of a VSDX diagram has changed a dashed line position.
*   Fixed: NullReferenceException occurred when creating an empty VSDX diagram.
*   Fixed: Argument out of range exception occurs while exporting a VSDX to PDF.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][1].
*   [Download Aspose.Diagram for .NET][2]
*   [Aspose.Diagram for .NET wiki docs][3] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][4] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Migrate from Earlier Versions of Aspose.Diagram API][7] - We keep track of Aspose.Diagram API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram
[2]: https://downloads.aspose.com/diagram
[3]: http://docs.aspose.com/display/diagramnet/Home
[4]: http://forum.aspose.com
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_diagram_NET
[7]: http://docs.aspose.com/display/diagramnet/Release+Notes




