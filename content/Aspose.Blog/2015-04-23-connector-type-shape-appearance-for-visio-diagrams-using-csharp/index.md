---
title: 'Connector Type Shape Appearance for Visio Diagrams using C#'
date: Thu, 23 Apr 2015 21:18:27 +0000
draft: false
url: /2015/04/23/connector-type-shape-appearance-for-visio-diagrams-using-csharp/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the new release version of [Aspose.Diagram for .NET][1] 5.2.0. With this new release, developers can now set the font directory paths for rendering in Visio diagrams and also they could set connector shape appearance. In addition to that we have added support to refresh milestones on the timeline shape and included another print method that takes printer and document name parameters on a customer request. It allows customizing document names during the print job. Besides the above new features, we also bring performance, formatting, and quality improvements in exporting Visio diagrams to any other supported formats.

## Specify Locations of Various Other Fonts

The operating systems store fonts in different folders and Aspose.Diagram looks for fonts in the respective Fonts folder. Developers can now specify locations of their own or third party fonts folders. Please refer to the following help topic: How to Specify TrueType Fonts Location

## Change the Connector Type Shape Appearance

Microsoft Office Visio offers connection types by going to the Design tab, and at the far left of the ribbon you can see Connectors in the Layout group. There are three types of Connectors in Visio: Right Angle, Straight Lines and curved, which can be found from the popup menu if you click the connectors button. This new release of the Aspose.Diagram APIs has included this feature support. Developers can now manage connector type shape's appearance programmatically. Following help topic shows, how developers can set appearance of the connector type shape: Set Appearance of the Connector Type Shape in Visio

## Refresh Milestones on the Timeline Shape

The timeline shape is the foundation to which we add the project milestones and events, Aspose.Diagram APIs allows to manage it. Using the older version, when we changed the period of timeline shape, milestones remain schedule based on the previous time period. To manage this thing, we have added a new RefreshTimeLine method in TimeLineHelper class. Following help topic shows, how developers can refresh milestones on the timeline shape: Refresh Milestones on the Timeline in Visio

## Setting Printer and Document Name in Print Job Queue

We have added another print method which sends print jobs to the printer. It takes printer and document name as parameters, so far users can customize the document name in job print queue. We have modified the following help topic: Printing a Diagram

In this recent release version, we have improved export areas regarding VSD to PDF, VSD to PNG, VSD to SVG and VSD to VDX. We have also included some fixes of manipulation. Please check a list of fixed issues below:

*   Fixed: VSDX to PDF conversion, incorrect rendering of the text items.
*   Fixed: VSD to PDF conversion, shapes are not properly visible.
*   Fixed: VSD to PNG conversion, shapes are not properly visible.
*   Fixed: VSD to SVG conversion, shapes are not properly visible.
*   Fixed: VSD to VDX conversion, shapes are not properly visible.
*   Fixed: VSD to VDX conversion, shape's text goes outside the border.
*   Fixed: Can't glue shape inside the container.
*   Fixed: Default date format is not available for Milestone shape.
*   Fixed: Default date format is not available for Timeline shape.
*   Fixed: Can't add shape second time in the same page or other one.
*   Fixed: Can't move shapes manually in Microsoft Office 2010/2013.
*   Fixed: Can't access shape ParaCollection objects.
*   Fixed: Argument Out of range error message occurred while placing a shape.
*   Fixed: Shape is using single connection point instead of different connection points.
*   Fixed: Warning message when opening resultant VDX diagram.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][2].
*   [Download Aspose.Diagram for .NET][3]
*   [Aspose.Diagram for .NET wiki docs][4] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/net
[2]: https://products.aspose.com/diagram
[3]: https://downloads.aspose.com/diagram/net
[4]: https://docs.aspose.com/diagram/net
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_diagram_NET




