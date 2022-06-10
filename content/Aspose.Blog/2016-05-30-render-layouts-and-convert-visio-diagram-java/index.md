---
title: 'Render Layouts and Convert Visio Diagram with Optimized Font Styles using Java'
date: Mon, 30 May 2016 05:20:56 +0000
draft: false
url: /2016/05/30/render-layouts-and-convert-visio-diagram-java/
author: Imran Rafique
summary: ''
tags: ['Convert Visio', 'Diagram Layout', 'Font Styles', 'Layout of the Shapes', 'Shape themes', 'VSDX to PDF', 'Visio shape formatting']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce that the new version 6.4.0 of [Aspose.Diagram for Java][1] API is now live. This version focuses on the conversion quality of Visio diagrams and mitigates the problems of altering the font name, font size, font style (bold, italic, underline), line style and so on. It also covers the aspects of partial rendering of the shape or losing the structure of the shapes in output diagram.

## Set Font Styles in Visio Export

The text items in the shape may have a font or other kind of formatting applied to it, such as bold or italic, which might change on exporting a Visio diagram to other supported file formats. We have tuned the behavior of font styles on saving, that helps in keeping all original formatting intact.

## Preserve the Original Layout in Visio Export

Upon changing the layout of shapes or simply converting the whole diagram, the lines may get routed differently. The dotted lines may appear as solid lines which will be the cause of confusion to distinguish between different types of objects. This version has also improved the layout algorithm to support different type of spaces and alignments. This helps to keep the original layout of the diagram unaltered.

Using Aspose.Diagram API, we have also improved the ability of writing VSDX diagram. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion, incorrect layout of the text in shapes.
*   Fixed: VSD to PDF conversion, the text of shapes is not bold.
*   Fixed: VSD to PDF conversion, the text of shapes is not italicized.
*   Fixed: VSD to PDF conversion, the font-size of the text in shapes is changed.
    
*   Fixed: Open and save routine of a VSDX diagram has lost theme of the shapes.
    
*   Fixed: Open and save routine of a VSDX diagram has lost the arrows of connectors.
*   Fixed: Open and save routine of a VSDX diagram has changed a dashed line position.
*   Fixed: NullReferenceException occurred when creating an empty VSDX diagram.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
*   [Download Aspose.Diagram for Java][3].
*   [Aspose.Diagram for Java wiki docs][4] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.

Intensity




[1]: https://products.aspose.com/diagram/java
[2]: https://products.aspose.com/diagram/java
[3]: https://downloads.aspose.com/diagram/java
[4]: https://docs.aspose.com/diagram/java
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_Diagram_Java




