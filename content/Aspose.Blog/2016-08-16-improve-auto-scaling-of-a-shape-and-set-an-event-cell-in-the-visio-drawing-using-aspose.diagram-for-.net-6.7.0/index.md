---
title: 'Improved Auto Scaling of a Shape and Set an Event Cell in the Visio Drawing using Aspose.Diagram for .NET 6.7.0'
date: Tue, 16 Aug 2016 22:58:19 +0000
draft: false
url: /2016/08/16/improve-auto-scaling-of-a-shape-and-set-an-event-cell-in-the-visio-drawing-using-aspose.diagram-for-.net-6.7.0/
author: Imran Rafique
summary: ''
tags: ['Auto scale a Visio shape', 'Event cells in Visio', 'Events Section', 'Set an event cell', 'Visio Shape']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We're pleased to announce that the [new version 6.7.0 of Aspose.Diagram for .NET API][2] is now live. It is a maintenance release with important bug fixes and improvements. With this release, we made several firm steps towards establishing the worth of import and render features of Visio diagrams. Using this new version 6.7.0, developers would be able to set an event cell in the Shapesheet as well as auto scaling a shape on adding its new instance in a Visio drawing. Developers can install an Aspose.Diagram Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][3]. We recommend our clients upgrade old version of Aspose.Diagram API to this latest one. For details on API fixes, please check Release Notes having a complete list of the features, enhancements and bug fixes.

## Setting Cells in the Event Section of ShapeSheet

The Microsoft Visio engine has many ways of triggering and responding to events. Users may put formulas into ShapeSheet cells that perform an action, such as running a macro or navigating to another drawing page, in response to an event. These formulas might be used in the Events section, which handles a group of events. Using Aspose.Diagram API, developers are already able to set various cells in the Event section of the ShapeSheet. However, this feature was not working properly for VSDM files. We have enhanced this feature to cover macro-enabled Visio formats. This help topic shows how to dynamically modify the event cells in Shapeheet: Setting Cells in the Event Section of ShapeSheet

## Auto Scale a Shape to Fit in the Visio Page

With the auto-scale capabilities, users may drag and drop a Visio shape on the drawing manually. Using Aspose.Diagram API, developers can now add this feature in their .NET applications. The AddShape method of Diagram class allows resizing shapes with auto-scale capabilities to fit in the whole page. In short, the auto-scaling capabilities of a Visio shape will be configured by the AddShape method of the Diagram class internally.

This version also addresses the issues of missing tables, appearance of the shapes, proper rendering of ActiveX button control and accuracy in size of the shapes. These enhancements and bug fixes improve performance and accuracy of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion - the red cross image appears instead of the shape.
    
*   Fixed: VSD to HTML conversion - the background color of the shape is not preserved.
    
*   Fixed: VSD to PDF conversion - the Color of the shapes are not preserved.
    
*   Fixed: VSD to PDF conversion - the table items are not preserved.
    
*   Fixed: Does not auto scale a shape on the drawing.
    
*   Fixed: Drags and drops the large size Visio shapes.
    
*   Fixed: Load and save routine of a VSDM diagram shows a cross sign in place of the button.
    
*   Fixed: Can't set an event cell of the shape in VSDM.
    
*   Fixed: VSD to PDF conversion - the logo transparency is not preserved.
    
*   Fixed: VSD to PDF conversion - incorrect line breaks in text.
    
*   Fixed: Junk reading of the angle property in a VSDX diagram.
    
*   Fixed: Incorrect readings of incoming nodes in a VSD diagram.
    
*   Fixed: A table is missing on converting a VSDX to PNG.
    
*   Fixed: Tables are missing on converting a VSDX to PNG.
    
*   Fixed: NullReferenceException occurred while saving a VSD to PDF.
    
*   Fixed: The gradient color pattern of a shape is changed on converting a VSD to PNG.
    
*   Fixed: The endpoints of connectors are not connected while saving in the VDX format.
    

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][4].
    
*   [Download Aspose.Diagram for .NET][5]
    
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][6] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][7] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
    
*   Migrate from Earlier Versions of Aspose.Diagram API - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.
    

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.

# Edit a Page-Level Comment in the Visio




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: http://www.aspose.com/downloads/diagram/net/new-releases/aspose.diagram-for-.net-6.7.0/
[3]: https://www.nuget.org/packages/Aspose.Diagram
[4]: https://products.aspose.com/diagram
[5]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[7]: https://blog.aspose.com/
[8]: https://github.com/asposediagram/Aspose_diagram_NET




