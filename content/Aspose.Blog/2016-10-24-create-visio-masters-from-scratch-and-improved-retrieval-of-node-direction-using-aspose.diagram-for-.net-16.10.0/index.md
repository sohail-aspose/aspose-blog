---
title: 'Create Visio Masters from Scratch using C# or VB.NET'
date: Mon, 24 Oct 2016 10:31:35 +0000
draft: false
url: /2016/10/24/create-visio-masters-from-scratch-and-improved-retrieval-of-node-direction-using-aspose.diagram-for-.net-16.10.0/
author: Imran Rafique
summary: ''
tags: ['Connector Direction', 'Create Master', 'Create Master from Scratch', 'Edit Master', 'Incoming and outgoing nodes', 'Visio Master']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce that the [new version 16.10.0 of Aspose.Diagram for .NET API][1] is now live. The new version of the API allows developers to create a master from scratch and include it in the Visio drawings. Developers can set an icon of the master to present data in the Visio drawings with graphics. Besides this, we have improved API to retrieve directions of all incoming and outgoing nodes as well as getting the relationship information between containers, lists, callouts, and member shapes. The recent version also covers a number of regular bug fixes and enhancements. Developers can install an Aspose.Diagram Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][2]. We recommend our clients upgrade old version of Aspose.Diagram API to this latest one. For details on API fixes, please check Release Notes having a complete list of the features, enhancements, and bug fixes.

## Create or Customize a Visio Master from Scratch using C#

Microsoft Office Visio provides a rich set of pre-made masters. We can drag a master on the Visio page, most of the resulting shapes will inherit their formulae and values from that master. In the past, our clients were placing shapes using stencil, drawing or template. Using version 16.10.0 or higher, they can now create a Visio master from scratch and it can be repeatedly used. This help topic shows how to create a master from scratch: Create Master from Scratch

\[gist id="cce69e51f567ea17ef24bc35fef0f689" file="Examples-CSharp-Load-Save-Convert-CreateMasterFromScratch-CreateMasterFromScratch.cs"\]

## Retrieve Incoming and Outgoing Nodes of the Shape

Aspose.Diagram API works with connected shapes in the Visio diagram. The developers use it to get structural information. We have enhanced this feature to unify the retrieval of incoming and outgoing nodes from each Visio drawing format.

This version also addresses the issues of misplaced shapes, additional content, the font formatting of shape and improper change in the shape size. These enhancements and bug fixes improve performance and accuracy of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion, the text of the shape appears not bold.
*   Fixed: Shape.GluedShapes method call is not returning all shape ID's.
*   Fixed: VSDX to PDF conversion, the connecting lines are not straight-I.
*   Fixed: VSDX to HTML conversion, the connecting lines are not straight-I.
*   Fixed: VSDX to PDF conversion, the connecting lines are not straight-II.
*   Fixed: VSDX to HTML conversion, the connecting lines are not straight-II.
*   Fixed: The text items are displaced on converting a VSDX to PDF.
*   Fixed: Missing the bold text formatting and incorrect line breaks on converting a VSDX to PDF.
*   Fixed: The incorrect position of text on converting a VSDX to PDF.
*   Fixed: The incorrect position of various text items on converting a VSDX to PDF.
*   Fixed: The vertical text appears as horizontal text on converting a VSDX to PNG.
*   Fixed: Retrieves reverse order of incoming and outgoing nodes from a VSDX.
*   Fixed: Can't retrieve relationships cell of the container shape from a VSD.
*   Fixed: The additional numbers are added while converting a VSD to SVG.
*   Fixed: The arrows are not being rendered correctly on converting a VSD to SVG.
*   Fixed: Incorrect rendering of the calendar on converting a VSD to SVG.
*   Fixed: Shape.ConnectedShapes method returns nodes with the reverse direction.
*   Fixed: Can't retrieve relationship cell of the shapes from a VSD.
*   Fixed: The background color of Visio pages is black on converting a VSD to SVG.
*   Fixed: Junk shape ID's are being retrieved from a VSD diagram.
*   Fixed: The incorrect symbol appears on converting a VSDX page to SVG.
*   Fixed: NullReferenceException occurred while converting a VDX to VSDX.
*   Fixed: The Page size option is being changed by setting the width and height of VSDM page.
*   Fixed: Can't retrieve relationship string of the shapes from a VSD.
*   Fixed: An argument error occurred while adding the ActiveX button.
*   Fixed: Improper change in size of a Visio shape on opening and saving in VSDM.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][3].
*   [Download Aspose.Diagram for .NET][4]
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   Migrate from Earlier Versions of Aspose.Diagram API - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.



[1]: http://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-16.10.0/
[2]: https://www.nuget.org/packages/Aspose.Diagram
[3]: http://www.aspose.com/products/diagram/net
[4]: http://downloads.aspose.com/diagram/net
[5]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family
[7]: https://github.com/asposediagram/Aspose_diagram_NET




