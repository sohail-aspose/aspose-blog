---
title: 'Removal of ICE_JNIRegistry.dll Dependency and Rendering Improvements with Aspose.Diagram for Java 3.0.0'
date: Thu, 30 Oct 2014 12:24:30 +0000
draft: false
url: /2014/10/30/removal-of-ice_jniregistry.dll-dependency-rendering-improvements/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Total Product Family', 'Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce the release of [Aspose.Diagram for Java][1] 3.0.0. With this release, we have removed the dependency on the ICE\_JNIRegistry.dll library. We used the library to load font information on Windows systems only. We have removed it to increase consistency and simplicity for developers. This release also improves rendering features by fixing error messages, bugs and including advanced techniques of enhancements.

## Removal of ICE\_JNIRegistry.dll Dependency

Previously, in the Aspose.Diagram for Java API, JNI was used to load font information on Windows systems. It was not compatible with Java Development Kit 7. We received a few requests from our customers to remove this dependency and are pleased to tell our customers that we have.

## Error Message Fixes and Other Rendering Improvements

This new release delivers improvements in rendering of properties, missing shapes, incorrect layouts and displacements of shapes. This release comprises a number of key fixes that help us improve rendering. This version also brings fixes to reported error messages and include various other enhancements as listed below:

*   Fixed: Action cells were not properly preview able in the Microsoft Office Visio 2013.
*   Fixed: Shape cut off when saving to VDX format.
*   Fixed: VSDX to PDF conversion - Adobe Acrobat error when opening PDF.
*   Fixed: VSDX to PDF conversion - shapes missing from the output PDF.
*   Fixed: VSDX to PNG conversion - horizontal lines missing from the output PNG.
*   Fixed: VSDX to PNG conversion - circular shapes missing from the output PNG.
*   Fixed: VTX to PDF conversion - null pointer exception when saving to PDF.
*   Fixed: Shape properties not added properly.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2]
*   [Download Aspose.Diagram for Java][3]
*   [Aspose.Diagram for Java docs][4] - help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, you can keep yourself updated with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/diagram/java
[2]: https://products.aspose.com/diagram/java
[3]: https://downloads.aspose.com/diagram/java
[4]: https://docs.aspose.com/diagram/java
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_Diagram_Java




