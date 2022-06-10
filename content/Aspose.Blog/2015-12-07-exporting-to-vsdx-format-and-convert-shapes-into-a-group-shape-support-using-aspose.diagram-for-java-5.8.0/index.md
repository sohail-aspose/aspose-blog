---
title: 'Exporting to VSDX Format and Convert Shapes into a Group Shape Support using Aspose.Diagram for Java 5.8.0'
date: Mon, 07 Dec 2015 05:36:18 +0000
draft: false
url: /2015/12/07/exporting-to-vsdx-format-and-convert-shapes-into-a-group-shape-support-using-aspose.diagram-for-java-5.8.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We're pleased to announce the new version 5.8.0 of the Aspose.Diagram for Java API. The support of exporting Visio diagrams to Microsoft Visio 2013 VSDX format has been added in this version. Developers can also create diagrams from scratch or modify the existing VSDX diagrams. Aspose.Diagram API now supports grouping a set of shapes and also save diagram into HTML without the toolbar. This release also includes the most recent bug fixes and enhanced retrieval of the diagram properties, layers visibility and auto shape positioning.

## Read and Write Microsoft Visio 2013 VSDX Format

In previous, we added support of reading VSDX diagram. Developers were able to read and extract the content of the diagram, but they were not able to save it in the VSDX format as well. From this version, they would also be able to write diagram in the VSDX format. Please also check this help topic: How to Save a Visio Diagram.

## Group a Set of Shapes Programmatically

Aspose.Diagram API has added support of grouping shapes together. The groups are a great way to organize shapes in a Visio drawing. Following help topic shows, how developers can group shapes together: Group Multiple Shapes Together in the Visio Drawing

## Save Visio Diagram into HTML without the Toolbar

In some use cases, our client's requirement was not to include toolbars in the resultant HTML document. In reference of this required feature, we have added the SaveToolBar property to the HTMLSaveOptions class. It specifies whether to include the toolbar or not. Following help topic shows, how developers can save diagram into the HTML format using SaveToolBar option: Specifying Diagram Save Options

Please check the newly added defect fixes and enhancements:

*   Fixed: Incorrect Visio page properties.
    
*   Fixed: DiagramSaveOptions.AutoFitPageToDrawingContent property works partially.
    
*   Fixed: Layers disappear when using setAutoFitPageToDrawingContent save option.
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new SaveToolBar option has been added to the HTMLSaveOptions class.
    
*   The VSDX format option has been added to the SaveFileFormat enum.
    
*   The group method has been added to the ShapeCollection class.
    

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
    
*   [Download Aspose.Diagram for Java][3].
    
*   Aspose.Diagram for Java wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java-e1401178596961.png "Aspose.Diagram for Java logo"
[2]: http://www.aspose.com/java/diagram-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/diagram-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_Diagram_Java




