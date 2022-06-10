---
title: 'Improved Rendering of Visio Drawings to PDF using Java'
date: Tue, 26 Aug 2014 09:32:10 +0000
draft: false
url: /2014/08/26/improved-rendering-of-visio-drawings-to-pdf-using-aspose.diagram-for-java-2.2.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


Today, we're pleased to announce the release of [Aspose.Diagram for Java][1] 2.2.0 as well as the goal of increasing consistency and simplicity for developers. The Aspose.Diagram API has improved export of Visio drawings to PDF format so that it exports just like Microsoft Visio does. Our development team has also worked to port the latest features from Aspose.Diagram .NET to Java and is pleased to make them available in the public API.

## Visio to PDF - Improvements

We have provided improved rendering support in this latest release. Normally, Microsoft Visio users prepare complex drawings in a beautiful layout. Chances are they’d like to maintain its appearance when exporting to PDF or any other supported formats. We have improved the API in this area. It's all based on the customer Visio drawing samples. This release includes a number of key fixes that help us improve Visio to PDF rendering:

*   The spaces between the text lines were messed up.
*   The computer symbol shape disappeared.
*   The text and image items were jumbled up.
*   Dotted lines were replaced with solid lines.
*   The page number sequence was incorrect.
*   The arrow thickness is preserved in the output PDF format. Previously, it was ignored.
*   Numbered items from the shape's text were missing.
*   A portion of the source PDF file was cut off.
*   The date was missing from the label shape.
*   The Microsoft Outlook icon was replaced by a Microsoft Word icon.
*   All the smiley faces were changed.
*   Hyperlinks were not preserved properly in the output PDF.
*   Some map shapes were missing.

## Error Message Fixes

This version brings fixes to reported error messages and include various other enhancements.

*   Fixed: the array index out of bound error message occurred while saving VSD to the PDF Format by calling the Diagram.Save method.
*   Fixed: the unknown source message occurred while converting VSD to PDF format.

## Auto-Ported Features from the .NET Version

Aspose.Diagram for Java is fully ported from the Aspose.Diagram for .NET API. The porting process has added a few more features that are already available in the latest version of Aspose.Diagram for .NET. Below is a of new features.

*   **Glue Shapes in Container using Connection Names** - There are many ways to glue shapes in the container, we've covered the basics of handling glue. Developers can now glue shapes in the container by passing connection name parameters. Previously, it was only possible by connection IDs. The new release of the Aspose.Diagram API has now made it very easy: just pass the exact connection name.  Developers can use either the connection IDs or name by using either the Page.glueShapesInContainer or Page.glueShapesInContainerByID methods. You can find the details of this feature in the following help topic: [Glue Shapes Inside the Container][2]
*   **Add Master to Diagram from Source Diagram** - This feature is useful primarily if we have added the new shapes and saved them to a source Microsoft Visio diagram. It helps developers to add a master to diagram from source diagram.  We have added a new overloaded Diagram.AddShape method. It takes a master name and a Diagram class object (the object that represents a Visio drawing). Please find details of this feature in the following help topic: [Add Master from the Stencil of Shapes][3]

## Public API Changes

The following API changes in the new version are also worth noting:

*   The Page.glueShapesInContainer and Page.glueShapesInContainerByID methods have been added. These methods take connection IDs or Name/NameU as parameters to glue shapes in the container.
*   The overloaded Diagram.addMaster method has been added. It takes a master name and the source diagram object as parameters.
*   The Page.addShape method has been added. It’s used to import a bitmap image as a Visio shape.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Hom][4][e][5][page for Aspose.Diagram for Java API][6]
*   [Download Aspose.Diagram for Java][7]
*   [Aspose.Diagram for Java wiki docs][8] - help documentation and API reference documents.
*   [Aspose.Diagram product family forum][9] - post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][10] - Don't limit yourself, you can keep yourself updated with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/java
[2]: https://docs.aspose.com/diagram/java/working-with-shapes-gluing/
[3]: https://docs.aspose.com/diagram/java/working-with-masters/#add-master-from-the-stencil-of-shapes
[4]: http://www.aspose.com/java/diagram-component.aspx
[5]: https://products.aspose.com/diagram/java
[6]: http://www.aspose.com/java/diagram-component.aspx
[7]: https://downloads.aspose.com/diagram/java
[8]: https://docs.aspose.com/diagram/java/
[9]: http://forum.aspose.com
[10]: https://blog.aspose.com/
[11]: https://github.com/asposediagram/Aspose_Diagram_Java




