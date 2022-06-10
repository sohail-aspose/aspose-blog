---
title: 'Visio Diagrams Formatting Improvements while Exporting to other File Formats in Aspose.Diagram for .NET 5.0.0'
date: Sun, 25 Jan 2015 01:30:01 +0000
draft: false
url: /2015/01/25/visio-diagrams-formatting-improvements-while-exporting-to-other-file-formats-in-aspose.diagram-for-.net-5.0.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We're pleased to announce the release of Aspose.Diagram for .NET 5.0.0. This is primarily a maintenance release. We address retaining text items formatting, shape's layout, shape color and missing shapes improvements. We also address about the fixes of assigning shapes to a layer, export performance and other error messages while loading diagrams or saving to any other supported formats.

## Layout Improvements in Visio Shapes

In some scenarios, the exported output files were not following the re-layout page options and placed at the same old locations. The list below describes shortlisted issues of this area:

*   Fixed: Laying out shapes in the FlowChart, the position of the shapes is not changed.
    
*   Fixed: VSD to PDF conversion, additional white space on the top of actual drawing.
    
*   Fixed: VSD to SVG conversion, incorrect visibility by overlapping of black color.
    

## Retain Shape Text Items Formatting and Color

The text that you move or copy have a font or other kind of formatting applied to it. The shapes were turned into the black shapes because the API exporter was not preserving fill color. Similarly, the incorrect sequence of line breaks, etc. It was the case with various Visio sample drawings. In this new release, we have included a few such fixes.

*   Fixed: VSDX to PDF conversion, incorrect sequence of line breaks in the shape's text.
    
*   Fixed: VSDX to HTML conversion, incorrect sequence of line breaks in the shape's text.
    
*   Fixed: VSD to PDF conversion, bullet text lines are going outside the container shape.
    
*   Fixed: VSD to HTML conversion, bullet text lines are going outside the container shape.
    
*   Fixed: VSD to PDF conversion, text items with incorrect position.
    
*   Fixed: VSD to PDF conversion, missing an empty line of the paragraph.
    
*   Fixed: VSDX to PDF conversion, missing textfield at the top right corner.
    
*   Fixed: VSD to PDF conversion, Shape's text with incorrect wrapping/layout.
    
*   Fixed: VSDX to PDF conversion, shape Fill color is changed.
    
*   Fixed: VSDX to HTML conversion, shape Fill color is changed.
    
*   Fixed: VSDX to PDF conversion, incorrect background color of the shapes.
    
*   Fixed: VSDX to HTML conversion, incorrect background color of the shapes.
    
*   Fixed: VSD to PDF conversion, background color of the shape is not preserved.
    

## Preserve missing shapes

In this release, we have also improved this area. We notice a few users were not able to preserve shapes in their output file formats. These issues have been fixed.

*   Fixed: VSDX to PDF conversion, shapes are not preserved.
    
*   Fixed: VSDX to HTML conversion, shapes are not preserved.
    

## Other Fixes

This new version brings fixes to reported error messages and include various other enhancements. Please see the complete list of fixed error messages in the new version.

*   Fixed: InvalidCastException message while saving diagram to SVG format.
    
*   Fixed: Error message when opened the output VDX drawing in the Visio.
    
*   Fixed: Warnings when opened the output Visio file in MS Office 2010/2007.
    
*   Fixed: VSDX to VDX conversion, warning message of invalid data.
    

In a scenario, the user was not able to assign shapes to a layer and facing export performance issue. We have fixed such issues too.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][2].
    
*   [Download Aspose.Diagram for .NET][3]
    
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: https://products.aspose.com/diagram
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_diagram_NET




