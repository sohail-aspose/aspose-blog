---
title: 'Retain Shadow on Converting Visio Shapes and Detect Glued or Connected Nature of Shapes using Aspose.Diagram for Java 6.0.0'
date: Tue, 02 Feb 2016 18:05:48 +0000
draft: false
url: /2016/02/02/retain-shadow-on-converting-visio-shapes-and-detect-glued-or-connected-nature-of-shapes-using-aspose.diagram-for-java-6.0.0/
author: Imran Rafique
summary: ''
tags: ['Aspose APIs', 'Aspose.Diagram for Java', 'Connect Visio shapes', 'Convert Visio', 'Glue Shapes', 'Imran.Rafique', 'Read VSSX stencil', 'Visio shape shadow', 'export VSSX']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We are happy to let our community know about the changes and newly offered features in our latest version 6.0.0 of the Aspose.Diagram for Java API. For developers, the newly added methods give programmatic access to detect the glued or connected nature of the two Visio shapes. The shadow effect adds a visual impact to the Visio shape. Aspose.Diagram API now supports retaining shadow when converting Visio shapes to any other supported format. Both these features help in giving the professional look to the resulting diagram. Besides this, we have improved VSSX stencil readings so that the developers could easily import shapes to fit obscure or specialized use cases. Many other recently reported defects and enhancements are included.

## Detecting Glue or Connect Nature of the Visio Shapes

Microsoft Office Visio allows users to glue or connect Visio shapes while creating a diagram. Developers can do the same programmatically using Aspose.Diagram API. In addition to that they can now detect connection nature like two shapes are glued or connected. To accomplish this task, it offers isGlued and isConnected methods in the Shape class. Both these methods take a destination shape object as a parameter and return resultant true or false. This help topic shows how developers can check whether two shapes are glued or connected: Verify Whether Two Visio Shapes are Connected or Glued

## Convert Visio with Shadow Effects of the Shapes

Using Aspose.Diagram API, users convert Visio diagrams to other supported formats. It also now transforms shadow effects of the shapes. Since users can now apply shadows to the shapes that help make the diagrams look more modern and attractive.

## Loading VSSX Stencil to Import Shapes

A VSSX file is a Visio stencil file. It saves a collection of shapes, connectors, or other objects that can be used within a drawing. Using Aspose.Diagram API, developers load VSSX stencil and then place shapes in their technical drawings. The loading part of the VSSX stencil file has been improved. Developers can now load even their complex Visio stencils.

Please check the newly added defect fixes and enhancements:

*   Fixed: VSD to VDX conversion, curve dynamic connectors turn into stright.
    
*   Fixed: Geometry of the connector shapes is incorrect.
    
*   Fixed: VSDX to EMF conversion - a zero bytes EMF file is generated.
    
*   Fixed: Copying a Visio diagram page operation does not preserve style of the shapes.
    
*   Fixed: Output formats PDF, EMF, JPEG, PNG, GIF, SVG, XPS, XAML and HTML - Copying Shape from the VSDX - an empty PDF is generated.
    
*   Fixed: Output format TIFF - Copying Shape from the VSDX - an error occurred.
    
*   Fixed: Copying a Visio diagram page does not preserve shapes completely.
    
*   Fixed: VSDX to TIFF conversion - an error occurred while saving into the Tiff format.
    
*   Fixed: VDX to VDX export, shape's text is not bold.
    
*   Fixed: VSD to VDX export, missing shadow of the shapes.
    
*   Fixed: Source VSD - ConnectCollection class returns additional connect and incorrect shape ids.
    
*   Fixed: Shape.connectedShapes method returns incorrect shape ids.
    
*   Fixed: Shape.gluedShapes method returns incorrect shape ids.
    
*   Fixed: Shape.connectedShapes method detects incorrect direction of the shape connectors.
    
*   Fixed: Bold style of text in a shape changes to normal while converting VSD to VDX.
    
*   Fixed: Output VSDX - A missing parts error occurred.
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   The isGlued method has been added in the Shape class.
    
*   The isConnected method has been added in the Shape class.
    

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
    
*   [Download Aspose.Diagram for Java][3].
    
*   Aspose.Diagram for Java wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for Java Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    
*   How to Migrate from Earlier Versions of Aspose.Diagram API – We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.
    

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java-e1401178596961.png "Aspose.Diagram for Java logo"
[2]: http://www.aspose.com/java/diagram-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/diagram-java/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_Diagram_Java




