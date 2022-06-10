---
title: 'Apply 3D Rotation Effects and Preserve SolutionXML Elements in Java'
date: Thu, 08 Jun 2017 00:08:16 +0000
draft: false
url: /2017/06/08/apply-3d-rotation-effects-and-preserve-solutionxml-elements-in-java/
author: Imran Rafique
summary: ''
tags: ['3D Rotation Cell values in Visio', 'Convert Visio to PDF', 'Fonts Substitution']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We are pleased to announce that the [new version 17.5 of Aspose.Diagram for Java API][1] is now live. The new version of the API has improved the storing and retrieval mechanism of SolutionXML elements. It also generates a warning about font substitution during the export of the drawing to PDF format. Developers can apply 3D rotation effects to Visio shapes with Aspose.Diagram API. All the regular bug fixes are also included. We recommend our clients [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. For details on API fixes, please visit the product Release Notes section of this new version.

## Get Notification of Fonts Substitution on Exporting Drawing to PDF

Aspose.Diagram API requires access to the accurate fonts in order to properly render the drawing to PDF format. It is possible that a font is used in a drawing, but not available on the machine. This will cause Aspose.Diagram API to render any instance of that font using the default font or the closest available font on the machine. The font substitution can change the look of the rendered PDF, developers may want to be notified when a font is missing and with what font it was replaced with. This help topic narrates how to get notification of font substitution on exporting Visio drawings into PDF format: [Receive Notification of Missing Fonts and Font Substitution during Export][3]

## Modify 3D Rotation Cell values in the Shapesheet

Users can modify cell values in "3D Rotation Properties" section of a shapesheet with Microsoft Visio application to apply 3D effects on a shape. From the recent version 17.5 or higher, developers would be able to incorporate this feature of retrieving and modifying cell values in "3D Rotation Properties" section in their Java applications. This help topic shows how to set 3D rotation cell values in the shapesheet: [3D Rotation Effects in a Visio Drawing][4]

Besides this, the mechanism of storing and retrieving SolutionXML elements from the Visio drawings has been improved because in various cases a simple open and save procedure was removing SolutionXML elements. The recent version also comprises a series of bug fixes.  In general, it improves the way of connecting shapes through the connection lines as well as preserves the color of shapes.

We auto port Aspose.Diagram for .NET to Java to give developers perfectly the same features on both platforms, so this version also incorporates the bug fixes and enhancements from its equivalent .NET version.

## Public API Changes

The following API changes in the new version are also worth noticing:

*   com.aspose.diagram.ThreeDFormat class has been added. It helps in retrieving and modifying 3D rotation cell values in the shapesheet.
*   WarningCallback member is added in com.aspose.diagram.saving.PdfSaveOptions class. It helps to implement an IWarningCallback interface to get notifications of font substitution.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][5].
*   [Download Aspose.Diagram for Java][6].
*   [Aspose.Diagram for Java wiki docs][7] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][8] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][9] - Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you will enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: http://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.5/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/diagram/java/aspose-diagram-font-operations/#receive-notification-of-missing-fonts-and-font-substitution-during-rendering
[4]: https://docs.aspose.com/diagram/java/3d-rotation-effects-in-a-visio-drawing/
[5]: https://products.aspose.com/diagram/java/
[6]: http://downloads.aspose.com/diagram/java
[7]: https://docs.aspose.com/diagram/java/
[8]: http://forum.aspose.com
[9]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[10]: https://github.com/asposediagram/Aspose_Diagram_Java




