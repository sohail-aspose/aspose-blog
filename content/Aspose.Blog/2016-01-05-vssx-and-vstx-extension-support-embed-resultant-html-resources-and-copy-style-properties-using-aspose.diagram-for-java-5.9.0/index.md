---
title: 'VSSX and VSTX Extension Support, Embed Resultant HTML Resources and Copy Style Properties using Aspose.Diagram for Java 5.9.0'
date: Tue, 05 Jan 2016 11:52:54 +0000
draft: false
url: /2016/01/05/vssx-and-vstx-extension-support-embed-resultant-html-resources-and-copy-style-properties-using-aspose.diagram-for-java-5.9.0/
author: Imran Rafique
summary: ''
tags: ['Aspose Java API', 'Aspose.Diagram', 'Copy Visio shapes', 'Imran.Rafique', 'VSDX', 'VSSX', 'VSTX', 'embed resultant HTML resources']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We are happy to let our community know about the changes and newly offered features in our latest version 5.9.0 of the Aspose.Diagram for Java API. The complete support for reading and writing VSSX stencil and VSTX template have been added. Developers can also embed output HTML resources into the single HTML document, copy styles and page sheet properties from other Visio drawings. This release also includes the most recent bug fixes and enhanced retrieval of the diagram properties, shapes visibility and auto shape positioning.

## Migrate from VSS and VST to VSSX and VSTX Formats

Starting from this version, Aspose.Diagram API allows developers to migrate their old stencils (.VSS) and templates (.VST) to the new VSSX and VSTX formats respectively. It helps in using vector graphics to create diagrams and get rid of old complex binary formats. Developers can do this task by simply running these lines of code:

```
// load an old VSS stencil
Diagram diagram = new Diagram(MyDir + "MyStencil.vss");
// save it in the VSSX format.
diagram.save(MyDir + "MyStencil.vssx", SaveFileFormat.VSSX);
```

## Embed Output HTML Resources and Save in a Stream

Aspose.Diagram API users can now serve the scenario where they need to embed output HTML resources into a single HTML document and also save it in the instance of a stream. This feature also enables them to store the output HTML in the repository or storage. Previously, Aspose.Diagram API was only saving the output HTML along with its resources in a separate directory. This help topic shows how developers can save the resulting HTML in the stream instance: How to Convert a Visio to HTML

## Copy Style and Formatting from another Visio

In Microsoft Office Visio, when we paste shapes into a destination Visio, it copies every style and formatting associated with the shapes. In order to mimic the behavior of MS Office Visio, Aspose.Diagram API has added CopyTheme method in the Diagram class and Copy method in the PageSheet class. These new methods also cover many defects in reference to missing style and formatting of the shapes during various manipulation tasks. This help topic shows how developers can copy a shape from another Visio: Copy Shapes from an Existing Visio

Please check the newly added defect fixes and enhancements:

*   Fixed: Shape.connectedShapes method is not working as expected.
    
*   Fixed: Shape.gluedShapes method is not working as expected.
    
*   Fixed: \[Output format VDX\] - Group Shape is not displayed properly.
    
*   Fixed: \[Output format HTML\] - Can't place a group shape from another Visio diagram.
    
*   Fixed: \[Output format PDF\] - Can't place a group shape from another Visio diagram.
    
*   Fixed: \[Output format VDX\] - Fill style of the Shapes is not preserved.
    
*   Fixed: VSDX to XPS conversion - an illegal error message occurred.
    
*   Fixed: Index out of bounds error occurred while loading a VSD diagram.
    
*   Fixed: VSD to VDX export, connectors position is changed.
    
*   Fixed: Open and save VSDX, the server shapes are missing.
    
*   Fixed: VDX to PDF export, the resultant PDF is blank.
    
*   Fixed: VDX to BMP export, a negative array size exception occurred.
    
*   Fixed: VDX to JPEG export, an argument exception occurred.
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   The VSSX format option has been added in the SaveFileFormat class.
    
*   The VSTX format option has been added in the SaveFileFormat class.
    
*   The VSTX format option has been added in the LoadFileFormat class.
    
*   The copyTheme method has been added in the Diagram class.
    
*   The copy method has been added in the PageSheet class.
    

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




