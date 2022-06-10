---
title: 'Control Image Brightness in Visio to Image and Edit Comments in Visio Diagrams using C#'
date: Mon, 07 Mar 2016 20:27:26 +0000
draft: false
url: /2016/03/07/convert-visio-to-image-with-image-brightness-settings-edit-comments-in-visio-csharp-asp.net/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to acknowledge the availability of new version 6.1.0 of the [Aspose.Diagram for .NET][1] API and let our community know about the progressions. The Aspose.Diagram API had already provided comprehensive and powerful functionalities to interact with Visio and automate regular drawing building and export tasks. In this progressive API version, we have enhanced **Visio to SVG** export, **Visio to image** export and editing Visio page level comment. We've squashed many other formatting bugs, error messages and incorporated the most suitable enhancements. We recommend you to upgrade their Aspose.Diagram API to this newer version. Let's get into the details.

## Visio to Image - Control Image Brightness

The brightness setting is handy when we convert Visio to an image because it controls the contrast performance of the various items. Aspose.Diagram API offers ImageBrightness property in the ImageSaveOptions class and it makes image quality the most ideal. We have applied internal optimizations to enhance it because its quality was not worthy, by one of our clients.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Load-Save-Convert-VisioSaveOptions-UseImageSaveOptions-UseImageSaveOptions.cs" >}}

Its help topic is already available here: [How to use Image Save Options][2]

## Visio to SVG - Preserves All Shape IDs

Many developers convert Visio drawing to SVG and use vector graphics in their web applications to show the technical diagrams in the web browser. Upon using previous versions of the Aspose.Diagram API, there was no way to track all shape IDs. Developers were unable to extract shapes uniquely from the SVG. So in the Aspose.Diagram API version 6.1.0 and later, developers would have the ability to parse SVG by unique shape IDs. This help topic shows how developers convert Visio to SVG: [How to Convert a Visio to SVG][3].

## Edit a Page-Level Comment in the Visio Diagrams

Each page can have its own set of page-level comments that are exhibited by an icon in the upper-left corner of the page. Aspose.Diagram API already allows developers to make a comment about the diagram, just add a comment by calling the AddComment method of the Page class which becomes a page-level comment. They can now edit a page-level comment.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-with-Comments-EditPageLevelCommentInVisio-EditPageLevelCommentInVisio.cs" >}}

This help topic shows how developers can edit a page-level comment: [Edit a Page-Level Comment in the Visio][4]

## Enhancements and Fixes

This API version also aims to ease the connection between multiple Visio shapes. In some reported use cases, the dynamic connectors were not being connected properly. We have raised the accuracy rate in extracting glued or connected shape IDs, missed or misplaced text and arrow of the shapes and preserve the color scheme of the shapes. All these factors give a professional look to the Visio diagrams. Please check a list of the resolved defects:

*   Fixed: VSD to PDF export - an extra word "text" is added in the shape's text.
*   Fixed: Incorrect setting of connector text location.
*   Fixed: VSD to VDX export - the dynamic connector is not being connected properly.
*   Fixed: VSDX to PDF and HTML export - missing shape's text item.
*   Fixed: VSDX to HTML and PDF export, the shape's text position is slightly misplaced.
*   Fixed: Shape.GluedShapes method returns incorrect shape IDs.
*   Fixed: VSD to HTML and PDF export - connector text items are misplaced.
*   Fixed: VSD to PDF export - the text items are missing.
*   Fixed: VSD to PDF export - the date strings turn into integer numbers.
*   Fixed: Can't preserve Name and NameU properties of the sub shapes.
*   Fixed: Missing attribute warning while loading the resultant VDX diagram.
*   Fixed: Shape.connectedShapes method does not detect some incoming shape ids.
*   Fixed: Saving in VDX - Duplicate of an element warning message.
*   Fixed: Saving in VDX - Can't connect two Visio shapes.
*   Fixed: VSD to PDF conversion - form tabs text is shifted down.
*   Fixed: VDX to VSDX export - the Null Reference Exception occurred.
*   Fixed: VSD to VDX export - the background text color of the shapes turns into black.
*   Fixed: VSD to VDX export - the arrows of the diagram are misplaced.
*   Fixed: VSD to VDX export - the text of the shapes goes outside the boundary.
*   Fixed: VSD to VDX export - ConnectCollection returns the incorrect count of the connects and values.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][5].
*   [Download Aspose.Diagram for .NET][6]
*   [Aspose.Diagram for .NET wiki docs][7] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][8] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][9] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   [How to Migrate from Earlier Versions of Aspose.Diagram API][11] - We keep track of Aspose.Diagram API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/net
[2]: https://docs.aspose.com/display/diagramnet/Save+a+Visio+Drawing#SaveaVisioDrawing-UseoftheImageSaveOptions
[3]: https://docs.aspose.com/display/diagramnet/How+to+Convert+a+Visio+Diagram#HowtoConvertaVisioDiagram-ExportaDiagramtoSVG
[4]: https://docs.aspose.com/display/diagramnet/Working+with+Comments#WorkingwithComments-EditaPage-LevelCommentintheVisioDiagram
[5]: https://products.aspose.com/diagram
[6]: https://downloads.aspose.com/diagram
[7]: http://docs.aspose.com/display/diagramnet/Home
[8]: http://forum.aspose.com
[9]: https://blog.aspose.com/
[10]: https://github.com/asposediagram/Aspose_diagram_NET
[11]: https://docs.aspose.com/display/diagramnet/Migrating+from+Earlier+Versions+of+Aspose.Diagram




