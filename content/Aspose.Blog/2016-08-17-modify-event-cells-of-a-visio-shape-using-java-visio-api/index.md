---
title: 'Modify Event Cells of a Visio Shape using Java'
date: Wed, 17 Aug 2016 11:50:57 +0000
draft: false
url: /2016/08/17/modify-event-cells-of-a-visio-shape-using-java-visio-api/
author: Imran Rafique
summary: ''
tags: ['Detect Visio File Type', 'Event Cells of a Shape', 'Modify Event Cells', 'Render a Visio diagram']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce that the [new version 6.7.0 of Aspose.Diagram for Java API][1] is now live. This release comes with a new feature, enhancements, and bug fixes. It gives a way to detect a Visio file format from an input stream. Developers would also be able to modify event cells of a Visio shape. Besides this, it covers many other regular bug fixes reported by our clients. We recommend our clients use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations. For details on API fixes, please visit the product Release Notes section of this new version.

## Detect Visio File Type from an InputStream

Aspose.Diagram API allows developers to determine the type of a Visio file from an input stream. Developers can already detect the type of a Visio file by passing a complete local file path which also includes the filename and extension. The detectFileFormat method of FileFormatInfo class now gives both options to pass a complete filename or an input stream of the Visio diagram. In short, there are two overloads of this method, the first one accepts a complete file name, while the second one accepts an input stream. This help topic shows how to programmatically detect the format of a Visio diagram: Detect the Format of Visio File Format from an InputStream

## Modify Event Cells of a Visio Shape

The ShapeSheet of a Visio shape has an Event section. The event section has event cells (TheText, EventDblCick, EventXFMod, EventDrop, EventMultiDrop, and TheDrop) in which formulas can be placed. These cells are being evaluated whenever an event occurs. We have enhanced the way of retrieving and updating the event cells in macro-enabled Visio file formats. This help topic shows how to dynamically modify the event cells in Shapeheet: Setting Cells in the Event Section of ShapeSheet

We auto port Aspose.Diagram for .NET to Java to give developers perfectly same features on both platforms, so this version also incorporates the bug fixes and enhancements from its equivalent .NET version. Please check a list of the resolved defects:

*   Fixed: VSD to PDF conversion - the red cross image appears instead of a shape.
*   Fixed: The endpoints of connectors are not connected when saving in the VDX format.
*   Fixed: Load and save routine of a VSDM diagram shows a cross in place of a button.
*   Fixed: Can't set an event cell of a shape in VSDM.
*   Fixed: Junk reading of an angle property in a VSDX diagram.
*   Fixed: Incorrect readings of incoming nodes in a VSD diagram.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
*   [Download Aspose.Diagram for Java][3].
*   [Aspose.Diagram for Java docs][4] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/diagram/java
[2]: https://downloads.aspose.com/diagram/java
[3]: https://downloads.aspose.com/diagram/java
[4]: https://docs.aspose.com/diagram/java
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_Diagram_Java




