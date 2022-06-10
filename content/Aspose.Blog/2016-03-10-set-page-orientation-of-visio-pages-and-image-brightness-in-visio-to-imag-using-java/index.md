---
title: 'Set Page Orientation and Image Brightness in Visio Diagrams using Java'
date: Thu, 10 Mar 2016 09:25:17 +0000
draft: false
url: /2016/03/10/set-page-orientation-of-visio-pages-and-image-brightness-in-visio-to-imag-using-java/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce the availability of new version 6.1.0 of the [Aspose.Diagram for Java][1] API and let our community know about the changes. This release has four noteworthy upgrades to Aspose.Diagram for Java API. It allows developers to set the orientation of the Visio page, protect the shape-ID attribute in SVG, manage the best image quality by setting its brightness level, and change comments on the Visio drawing page. Below, we list some major enhancements and other defect fixes. Let's go into the details.

## Set Page Orientation in Visio using Java

Microsoft Office Visio allows users to rotate the page from portrait to landscape or landscape to portrait. Aspose.Diagram API gives automatic access to accomplish the task and even developers can set the orientation the same as on the printer. PrintPageOrientation class of the Aspose.Diagram API allows us to do so. Previously, this feature was not working as expected. So, in the Aspose.Diagram API version 6.1.0 and later, developers would be able to set the page orientation. This help topic shows how developers can set the Visio page orientation: [Set Orientation of the Visio Page][2]

{{< gist aspose-diagram 92a05cb833bad6d60de2968c96b40ee4 "Examples-src-main-java-com-aspose-diagram-examples-Pages-SetVisioPageOrientation-SetVisioPageOrientation.java" >}}

## Edit Brightness While Converting Visio Drawing to Image

Modifying an image's brightness allows to change the general measure of light in an image. It controls the contrast between the light and dull areas of an image. Aspose.Diagram API offers ImageBrightness property in the ImageSaveOptions class to lead the best image quality. We have applied internal optimizations to enhance it. Its help topic is already available here: How to use Image Save Options

{{< gist aspose-diagram 92a05cb833bad6d60de2968c96b40ee4 "Examples-src-main-java-com-aspose-diagram-examples-LoadSaveConvert-VisioSaveOptions-UseImageSaveOptions-UseImageSaveOptions.java" >}}

## Visio to SVG - Export Maps Shape-ID Attribute

Many of our clients use Aspose.Diagram API to convert a Visio drawing to SVG as it can be dynamic and interactive. The SVG is natively supported by most modern browsers and is broadly accessible on mobile devices. Using the old API versions, there was no way to distinguish shapes by their IDs. We have mapped the shape id attribute in SVG. Developers can use the recent version 6.1.0 or higher for this purpose. This help topic shows how developers convert Visio to SVG: [How to Convert a Visio to SVG][3]

## Change Comment on the Visio Page

We add comments in the Visio diagrams to give additional and more detailed information. The Visio page level comment is one way of addressing the page part of the drawing. Aspose.Diagram API has the support of adding a page-level comment. Developers can also change the existing page level comments. This help topic shows how developers can edit a page-level comment: [Edit a Page-Level Comment in the Visio][4]

Many other formatting imperfections, error messages of the Visio drawing structures, and additional entry problems have been fixed. It also moves the misplaced entries to their proper location. Please check the newly added defect fixes and enhancements:

*   Fixed: VSD to PDF conversion, the word "text" is added in the shape's text.
*   Fixed: Incorrect setting of connector text location.
*   Fixed: Warning of the missing attribute when opened the resultant VDX diagram.
*   Fixed: Shape.connectedShapes method does not detect some incoming shape ids.
*   Fixed: Output VDX - Duplicate of an element warning message.
*   Fixed: VSD to VDX export - the background text color of the shapes turns into black.
*   Fixed: VSD to VDX export - the arrows of the diagram are misplaced.
*   Fixed: VSD to VDX export - the text of the shapes goes outside the boundary.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][5].
*   [Download Aspose.Diagram for Java][6].
*   Aspose.Diagram for Java wiki docs - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][7] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][8] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [How to Migrate from Earlier Versions of Aspose.Diagram API][10] – We keep track of Aspose.Diagram API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/java
[2]: https://docs.aspose.com/display/diagramjava/Set+Orientation+and+Control+the+Export+of+Hidden+Visio+Pages+on+Saving
[3]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[4]: https://docs.aspose.com/display/diagramjava/Working+with+Comments
[5]: https://products.aspose.com/diagram/java
[6]: https://downloads.aspose.com/diagram/java
[7]: https://forum.aspose.com/
[8]: https://blog.aspose.com/
[9]: https://github.com/asposediagram/Aspose_Diagram_Java
[10]: https://docs.aspose.com/display/diagramjava/Migrating+from+Earlier+Versions+of+Aspose.Diagram+for+Java




