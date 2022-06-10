---
title: 'Display Property Values of the Shape on Visio Drawing and Create a Master Shape from Scratch in Java'
date: Wed, 26 Oct 2016 09:55:14 +0000
draft: false
url: /2016/10/26/display-property-values-of-the-shape-on-visio-drawing-and-create-a-master-shape-from-scratch-using-aspose.diagram-for-java-16.10.0/
author: Imran Rafique
summary: ''
tags: ['Create Master Shape', 'Create Master Shape of Visio Drawing in Java', "Display Shape's Property on Drawing"]
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce that the [new version 16.10.0 of Aspose.Diagram for Java API][1] is now live. The new version of the API allows to automatically change the display text of Visio drawing from Data1, Data2, and Data3 properties. Developers can even formulate a shape text from another shape's properties. Developers can also create a master shape from scratch or edit an existing master shape in the Visio drawings. They can set all basic properties and icon of the master shape. We recommend our clients [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. For details on API fixes, please visit the product Release Notes section of this new version.

## Display Data1, Data2 and Data3 Property Values on Visio Drawing

Using Aspose.Diagram API, developers may set a shape's Data1, Data2, and Data3 properties. On populating a shape's text from these properties, Aspose.Diagram API was not automatically modifying the text of the various shapes in Visio drawing. Although, it was updating property values in the Shapesheet. We have enhanced this feature similar to the behavior of Microsoft Office Visio. It now automatically modifies the text of shape even if we populate the text of a shape from another shape's properties.

## Create or Customize Master Shape from Scratch

Users can manually drag and drop a shape from stencil to a Visio page. During this process, Microsoft Office Visio copies the master shape into the local document stencil before the first instance is positioned on the page. The actual shape that is seen in the page inherits most of its attributes from its master. Using Aspose.Diagram API, developers can now manage to create a master shape from scratch. They might also edit an existing master shape. This help topic shows how to create a master from scratch: Create Master from Scratch

We auto port Aspose.Diagram for .NET to Java to give developers perfectly the same features on both platforms, so this version incorporates the bug fixes and enhancements from its equivalent .NET version. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion - shapes are missing.
*   Fixed: VSD to PDF conversion, the text of the shape appears not bold.
*   Fixed: Shape.GluedShapes method call is not returning all shape ids.
*   Fixed: The vertical text appears as horizontal text on converting a VSDX to PNG.
*   Fixed: The appearance of shapes is changed while converting a VSDX to PNG.
*   Fixed: The incorrect symbol appears on converting a VSDX page to PNG.
*   Fixed: The number format error occurred on saving a VST to PNG.
*   Fixed: The number format error occurred on saving a VST to PDF.
*   Fixed: Retrieves reverse order of incoming and outgoing nodes from a VSDX.
*   Fixed: Can't retrieve relationships cell of the container shape from a VSD.
*   Fixed: A Number Format error occurred on converting a VSD to SVG.
*   Fixed: The black color rectangles are generated on converting a VSD to SVG.
*   Fixed: The arrows are not being rendered correctly on converting a VSD to SVG.
*   Fixed: The text items are displaced on converting a VSD to SVG.
*   Fixed: Incorrect rendering of the calendar on converting a VSD to SVG.
*   Fixed: Shape.connectedShapes method returns nodes with the reverse direction.
*   Fixed: Can't retrieve relationship cell of the shapes from a VSD.
*   Fixed: The background color of Visio pages is black on converting a VSD to SVG.
*   Fixed: Junk shape ID's are being retrieved from a VSD diagram.
*   Fixed: The incorrect symbol appears on converting a VSDX page to SVG.
*   Fixed: The Page size option is being changed by setting the width and height of the VSDM page.
*   Fixed: Can't retrieve relationship string of the shapes from a VSD.
*   Fixed: Improper change in the size of a Visio shape on opening and saving in VSDM.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][3].
*   [Download Aspose.Diagram for Java][4].
*   [Aspose.Diagram for Java wiki docs][5] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [Migrate from Earlier Versions of Aspose.Diagram API][9] – We keep track of Aspose.Diagram API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: http://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-16.10.0/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: http://www.aspose.com/products/diagram/java
[4]: http://downloads.aspose.com/diagram/java
[5]: http://docs.aspose.com/display/diagramjava/Home
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family
[8]: https://github.com/asposediagram/Aspose_Diagram_Java
[9]: http://docs.aspose.com/display/diagramjava/Migrating+from+Earlier+Versions+of+Aspose.Diagram+for+Java




