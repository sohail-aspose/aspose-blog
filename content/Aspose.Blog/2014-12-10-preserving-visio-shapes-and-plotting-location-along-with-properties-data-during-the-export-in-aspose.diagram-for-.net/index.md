---
title: 'Preserve Visio Shapes and Plot Location using Aspose.Diagram for .NET 4.6.0'
date: Wed, 10 Dec 2014 15:07:39 +0000
draft: false
url: /2014/12/10/preserving-visio-shapes-and-plotting-location-along-with-properties-data-during-the-export-in-aspose.diagram-for-.net/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the release of Aspose.Diagram for .NET 4.6.0. We frequently release new versions with recent breakthroughs, API operation advancements, and feature operation news. In this blog post, we address many rendering, accurate layout and export issues that were reported for export PDF, HTML and other supported formats in earlier versions. Similarly, there is a list of other issues fixed in this release.

## Plotting Location and Style of Visio Shapes

In some scenarios, the exported output files were missing a few types of shapes or rendering incomplete shapes. Similarly, the shapes were turned into the black shapes because the API exporter was not preserving fill color. It was the case with various Visio sample drawings. The list below describes shortlisted issues of this area:

*   Fixed: VSDX to HTML conversion, circle shapes turned into black shapes.
*   Fixed: VSDX to PDF conversion, circle shapes turned into black shapes.
*   Fixed: VSDX to PDF conversion, all shapes turned into black shapes.
*   Fixed: VSDX to HTML conversion, all shapes turned into black shapes.
*   Fixed: VSDX to PDF conversion, the shape fill color is not preserved.
*   Fixed: VSDX to PDF conversion, the arrow shapes are not preserved.
*   Fixed: Half visibility of second "Interface Normal" shape.
*   Fixed: VSDX to HTML conversion, the arrow shapes are not preserved.
*   Fixed: Can't set the Visio drawing's page route style.
*   Fixed: Layer visibility is false (VSDX), but its shapes are present in the output PNG file.

## Importing Shapes and their Property Data

There was no way to add a few shapes from a stencil file. In another scenario, users were not able to add or update shape property data because the API importer was not doing so. We have fixed these issues in the new version.

*   Fixed: Can't add "Vlan Interface" shape from the stencil file.
*   Fixed: Can't add "Interface Normal" shape from the stencil file.
*   Fixed: Adding two shape data properties, but only one is visible in the Microsoft Office Visio.
*   Fixed: VSD to PDF conversion, can't update Visio document properties.
*   Fixed: VSDX to PDF conversion, can't update Visio document properties.
*   Fixed: Shape names are changed when added a group shape.

## Organizing Visio Shapes

Aspose.Diagram API has already supported gluing shapes inside the container.  In this release, we have also improved this area. We notice a user was not able to organize shapes inside the specific container. This issue has been fixed.

## Removal of Additional White Space and Shapes

During the export of Visio files to PDF or thumbnail format, the Aspose.Diagram API exporter was placing a few additional white space around the actual drawing or extra half ellipse shape.

*   Fixed: VSD to PDF export, extra white space on the left and right side of the drawing.
*   Fixed: VSD to PNG export, extra white space on the left and right side of the drawing.
*   Fixed: VSD to pdf conversion, extra half ellipse type shapes are generated.

## Other Fixes

This new version brings fixes to reported error messages and include various other enhancements. Please see the complete list of fixed error messages in the new version.

*   Fixed: Verification failed of a PDF/A-1b file with Adobe Acrobat Pro X.
*   Fixed: VTX to PDF conversion, Unable to cast object error message.
*   Fixed: Control whether the shape is added as a 1D or 2D shape.
*   Fixed: Add a constructor of Window class.
*   Fixed: VSD to SVG conversion, shapes with the hyperlink is not preserved.
*   Fixed: VSDX to PDF conversion, the value of title field is missing.
*   Fixed: VSD to VDX export, the flag shape appears messed up.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][1].
*   [Download Aspose.Diagram for .NET][2]
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][3] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][4] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][5] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[4]: https://blog.aspose.com/
[5]: https://github.com/asposediagram/Aspose_diagram_NET




