---
title: 'Retrieve Glued Visio Shape ID using C# with Aspose.Diagram'
date: Thu, 07 Apr 2016 15:50:37 +0000
draft: false
url: /2016/04/07/retrieve-glued-visio-shape-id-using-csharp/
author: Imran Rafique
summary: ''
tags: ['Glue Visio shapes', 'Visio diagram properties', 'Visio page orientation', 'Visio shape colors', 'Visio shape connects', 'Visio shape hyperlink', 'Visio shape styles']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the availability of new version 6.2.0 of the [Aspose.Diagram for .NET][1] API. This version makes some nice improvements and gives accuracy in retrieving the glued Visio shape ID as well as improves manipulations associated to apply formatting in the whole diagram when converting to any supported format. This version also incorporates several tweaks and bug fixes reported in the Aspose forums. We're truly thankful to our Aspose worldwide community that is the heartbeat of everything.

## Enhanced Retrieval of the Glued Shapes in Visio Diagrams

Aspose.Diagram API offers a GluedShapes method in the Shape class which returns an array that contains the IDs of the shapes that are glued to a shape. All incoming and outgoing nodes could be identified. In some reported use cases, clients were not able to identify incoming and outgoing nodes because of the duplicate and incorrect shape IDs being retrieved. This version covers fixes of these defects.

## Quality Export Rendering of the Visio Diagrams

Many of our clients convert Visio drawings to any other file type supported by Aspose.Diagram API and report their problematic Visio samples where they're facing the problems like the wrong line breaks in the shape's text, displaced shapes, missing shapes, duplications in the text items, incorrect font alignment, changes in the shape appearance, diagram properties are not being preserved and many more. In this version, we have fixed a large number of such problems. All these factors give an excellent look to the Visio diagrams. Please check a list of the resolved defects:

*   Fixed: VSD to VDX export is missing or misplacing text items.
*   Fixed: VSD to PDF export adds a text "options" in the form menu.
*   Fixed: VSDX to HTML export misplaces the text item of the shape.
*   Fixed: VSDX to PDF export - the circular shape's boundary is not visible.
*   Fixed: VSDX to PDF export - the button shape does not have a boundary and fill color.
*   Fixed: VSDX to PDF and HTML exports - the shape's text position is slightly misplaced.
*   Fixed: VSDX to HTML export - the circular shape's boundary is not visible.
*   Fixed: VSDX to HTML export - the button shape does not have a boundary and fill color.
*   Fixed: VSD to PDF export - the shape's text goes outside the boundary.
*   Fixed: VSD to HTML export - the text items of shapes are not aligned at the center.
*   Fixed: VSD to VDX export - an invalid resultant file is created.
*   Fixed: VSD to VDX export misses display text of the Bitmap shapes.
*   Fixed: VSDX to VDX export - the appearance of the shapes is changed.
*   Fixed: Can't change page orientation by setting PrintPageOrientation property.
*   Fixed: The signature of Aspose.Diagram for .NET 6.1.0 MSI is corrupt or invalid.
*   Fixed: VSDX to PDF export - the green color is applied on the shape's boundary.
*   Fixed: VSD to VSDX export - Diagram.DocumentProps.Manager returns an empty string.
*   Fixed: VSDX to JPEG export - an empty margin is generated on the left side.
*   Fixed: VDX to VSDX export generates a corrupt output file.
*   Fixed: VSD to PDF export renders an incorrect hyperlink address.
*   Fixed: VSD to PDF export renders incorrect formatting of the bullets.
*   Fixed: VSD to PDF export includes an extra word in the shape's text.
*   Fixed: VSD to HTML export includes an extra word in the shape's text.
*   Fixed: Diagram exception occurred while loading VSDX file.
*   Fixed: An argument exception occurred when saving diagram in the VSDX.
*   Fixed: VSD to SVG export - an arithmetic overflow error occurs.
*   Fixed: VSDX to PDF export - Key parameter can't be null error message occurred.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][2].
*   [Download Aspose.Diagram for .NET][3]
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   How to Migrate from Earlier Versions of Aspose.Diagram API - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/net
[2]: https://products.aspose.com/diagram
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_diagram_NET




