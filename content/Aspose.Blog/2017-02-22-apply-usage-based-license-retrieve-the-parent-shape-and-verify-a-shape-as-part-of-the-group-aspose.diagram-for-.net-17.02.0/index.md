---
title: 'Apply Usage Based License, Retrieve the Parent Shape and Verify a Shape as Part of the Group using Aspose.Diagram for .NET 17.02.0'
date: Wed, 22 Feb 2017 19:13:07 +0000
draft: false
url: /2017/02/22/apply-usage-based-license-retrieve-the-parent-shape-and-verify-a-shape-as-part-of-the-group-aspose.diagram-for-.net-17.02.0/
author: Imran Rafique
summary: ''
tags: ['Aspose Licensing Model', 'CLS compliant', 'Group Shape', 'Parent Visio Shape', 'Usage Based License']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We're pleased to announce that the [new version 17.02.0 of Aspose.Diagram for .NET API][2] is now live. The new version of the API adds four new features. Developers can apply usage based license to Aspose.Diagram assembly. The new licensing mechanism will be used along with the existing licensing method. Our clients who want to be billed based on the usage of the API features can use the metered licensing. Developers can also retrieve the parent shape on manipulating the recent shape as well as verify a shape, whether it is a part of any group shape. Aspose.Diagram API is now marked as CLS compliant. It ensures that the Aspose.Diagram assembly can be used from any CLR language. The recent version also covers a number of regular bug fixes and enhancements. Developers can install an Aspose.Diagram Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][3]. We recommend our clients upgrade old version of Aspose.Diagram API to this latest one. For details on API fixes, please check Release Notes having a complete list of the features, enhancements and bug fixes.

## Usage Based Licensing ModelThe new version 17.02.0 of Aspose.Diagram API provides a Metered class. It allows developers to set public and private keys to apply usage based license by calling a SetMeteredKey method of the Metered class. The metered licensing system monitors the regular usage of Aspose.Diagram API and keep track of the Aspose API licenses. Please check this help topic to know the implementation of metered license: [Set Public and Private Keys to Apply Metered License][4]

## Retrieve the Parent Visio Shape of Recent Sub-ShapeA group shape contains multiple sub-shapes. The sub-shape references cells of the parent shape. Using Aspose.Diagram API, developers can now track the parent shape of recent sub-shape. It was a demanded feature to retrieve the shape hierarchy from bottom to top level. In the past, developers were only able to get the shapes from its parent shape. They can now go a level back. This help topic shows how to retrieve the parent shape of recent sub-shape: [Retrieve the Parent Shape of a Sub-Shape][5]  

## Verify Whether the Visio Shape is Part of any Group ShapeAspose.Diagram API has support to group multiple shapes together in a Visio drawing. Developers can now apply a check in the code, whether the recent shape is part of any group shape or not. This feature is handy to prepare use cases for building complex Visio drawings. This help topic shows how to verify whether the recent shape is part of any group shape: [Verify Whether the Visio Shape is in a Group of Shapes][6]  
  
The recent version also incorporates the fixes of rendering incorrect color of shapes, formatting incorrections, partial rendering of shapes and errors on loading Visio drawings. These enhancements and bug fixes improve performance and accuracy of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion, the background color shade of a group shape is getting changed.
    
*   Fixed: VSDX to PDF conversion, incorrect background color of the shape.
    
*   Fixed: The border lines of the table are missing on converting a VSDX to PNG.
    
*   Fixed: The text items are not aligned properly on converting a VSDX to PNG.
    
*   Fixed: Rendering incorrect color of shapes on converting a VSD to PNG.
    
*   Fixed: HTMLSaveOptions.DefaultFont property does not work as expected.
    
*   Fixed: The color of shapes is not being rendered correctly on converting a VSD to HTML.
    
*   Fixed: The wrong text alignment of shapes on saving in EMF.
    
*   Fixed: The rounded shape corners are being changed on converting a VSD to PDF.
    
*   Fixed: The layout of dynamic arrow connector is changed on converting a VSD to PDF.
    
*   Fixed: The Visio shapes are displaced on converting a VSDX to PDF.
    
*   Fixed: The vertical text appears as horizontal text on converting a VSDX to PDF.
    
*   Fixed: Vertical text box is overhanging the edge of the node while export of VSDX to PDF.
    
*   Fixed: An error occurred in loading a VSDX diagram.
    
*   Fixed: Can't access file error occurred on converting a VSDX to HTML.
    
*   Fixed: NullReferenceException at Diagram.Save while converting VSD to HTML.
    
*   Fixed: NullReferenceException at Diagram.Save when CustomProp.Name property is not set.
    

## Aspose.Diagram for .NET ResourcesThe following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][7].
    
*   [Download Aspose.Diagram for .NET][8]
    
*   Diagram for .NET wiki docs- Help documentation and API reference documents.
    
*   [Diagram product family forum][9]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][10]\- Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Diagram for .NET Examples][11]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
    

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: http://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.02.0/
[3]: https://www.nuget.org/packages/Aspose.Diagram
[4]: https://docs.aspose.com/display/diagramnet/Licensing#Licensing-SetPublicandPrivateKeystoApplyMeteredLicense
[5]: https://docs.aspose.com/display/diagramnet/Add%2C+Retrieve%2C+Copy+and+Read+Visio+Shape+Data#Add,Retrieve,CopyandReadVisioShapeData-RetrievetheParentShapeofaSub-Shape
[6]: https://docs.aspose.com/display/diagramnet/Group%2C+Convert+and+Verify+Shapes#Group,ConvertandVerifyShapes-VerifyWhethertheVisioShapeisinaGroupofShapes
[7]: http://www.aspose.com/products/diagram/net
[8]: http://downloads.aspose.com/diagram/net
[9]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[10]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[11]: https://github.com/asposediagram/Aspose_diagram_NET




