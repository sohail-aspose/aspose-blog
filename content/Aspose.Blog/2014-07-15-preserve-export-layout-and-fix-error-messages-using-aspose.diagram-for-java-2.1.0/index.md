---
title: 'Preserve Export Layout and Fix Error Messages using Aspose.Diagram for Java 2.1.0'
date: Tue, 15 Jul 2014 10:42:04 +0000
draft: false
url: /2014/07/15/preserve-export-layout-and-fix-error-messages-using-aspose.diagram-for-java-2.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We are pleased to announce the release of Aspose.Diagram for Java 2.1.0. This release fixes issues primarily related to the measurement of elements and export layout quality of Microsoft Visio drawings. These formatting improvements make it easy to create good-looking output PDFs with just a couple of lines of source code. This release also covers a number of new error messages, enhancements along with bug fixes.

## Export Layout Quality and Improvements

If  your Microsoft Visio users have prepared a pretty heavy drawing in a beautiful layout, chances are they’d like to maintain its appearance when exporting it to other formats. We have improved the APIs performance in this area. This release includes a number of key fixes when exporting Visio diagram to the PDF format:

*   The arrow thickness is preserved in the output PDF format. Previously, it was ignored.
    
*   The caption text gets overlapped with the arrow symbol line. It is now fixed.
    
*   The black spots were generated in the output PDF format. The heading row in table and other icons at the bottom were getting blackened.
    
*   Pop up message was appearing as "Do you want to save changes to 'MyDigram.pdf' before closing?" while closing output PDF documents.
    

## Error Message Fixes

This new version brings fixes to reported error messages and include various other enhancements. Please see the complete list of fixed error messages in the new version.

*   Fixed: NumberFormatException message when calling the Page.addShape method.
    
*   Fixed: IllegalArgumentException message occurred when converting VSD to PDF format.
    
*   Fixed: NumberFormatException message when saving SVG format
    

## Other Auto-Ported Features from the .NET Version

Aspose.Diagram for Java is fully ported from the Aspose.Diagram for .NET API. The porting process has added a few more features that are already available in the latest version of Aspose.Diagram for .NET. Below is a of new features.

*   **Get a master from a Microsoft Visio drawing by name** - Developers can now retrieve a master object using its name. The MasterCollection.getMasterByName method searches all masters in the masters collection’s containing master. Developers just need to pass the exact master name. Developers can use either the master ID or name: the MasterCollection.GetMaster and MasterCollection.GetMasterByName methods give developers that option. You can find the details of this feature in the following help topic: Get Master from a Visio Drawing by Name
    
*   **Glue group shapes inside a container** - Developers can dynamically glue group shapes inside the container group shape. You can find details of this feature in the following help topic: Glue Shape Inside a Container
    
*   **Check for the presence of master in a Visio drawing by name** - Developers can now check the presence of a master object by its name using the MasterCollection.IsExist method. It checks that the title master exists and, if it does, returns true, otherwise false. Developers can use either the master ID or name: the MasterCollection.IsExist method supports both options. You can find details of this feature in the following help topic: Check Presence of a Master in a Visio Drawing
    
*   **Glue Visio shapes together with connection points** - This feature allows developers to glue shapes together with connection points. A connection point is a special point on a shape that can be used to “glue” other shapes to it. When developers glue a shape to a connection point, the shapes stay connected, even if one of the shapes is moved. Please see this feature in the following help topic: Glue Visio Shapes Together with Connection Point
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   The MasterCollection.GetMasterByName method has been added. It takes a master name as parameter and returns a master object.
    
*   The MasterCollection.IsExist method has been added. It takes a master ID or name as parameter and returns true in case the master is present.
    
*   The Page.GlueShapesInContainer method has been added. It’s used to glue shapes in the container.
    
*   The Page.GlueShapes method has been added. It takes three parameters.
    
    *   long shapeFromId or Shape shapeFrom
        
    *   ConnectionPointPlace placeTo
        
    *   long shapeToId or Shape shapeTo
        

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2]
    
*   [Download Aspose.Diagram for Java][3]
    
*   Aspose.Diagram for Java wiki docs - help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java-e1401178596961.png "Aspose.Diagram for Java logo"
[2]: http://www.aspose.com/java/diagram-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/diagram-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_Diagram_Java




