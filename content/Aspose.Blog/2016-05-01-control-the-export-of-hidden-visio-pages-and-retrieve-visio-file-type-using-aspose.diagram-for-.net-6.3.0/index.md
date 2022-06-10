---
title: 'Control the Export of Hidden Visio Pages and Retrieve Visio File Type using Aspose.Diagram for .NET 6.3.0'
date: Sun, 01 May 2016 15:35:37 +0000
draft: false
url: /2016/05/01/control-the-export-of-hidden-visio-pages-and-retrieve-visio-file-type-using-aspose.diagram-for-.net-6.3.0/
author: Imran Rafique
summary: ''
tags: ['Arabic Text rendering', 'Detect Visio File Type', 'Hebrew text rendering', 'Hide page in Visio', 'Visio shape formatting', 'export hidden Visio page']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We're pleased to announce that the new version 6.3.0 of Aspose.Diagram for .NET API is now live. This new version brings a number of new features, enhancements and bug fixes. This version gives access to the developers to control the export of Hidden Visio pages in output files. Developers may also detect the Visio file type by its content and export diagrams with Arabic and Hebrew text. All this is achievable with Aspose.Diagram API.

## Include or Exclude Hidden Pages of Visio on Saving to SVG, XPS, Image, HTML and PDF

Using Aspose.Diagram API, developers may hide the page of a Visio diagram through the cell UIVisibility in the page ShapeSheet yet they were not able to exclude the hidden pages on saving to output files. This version gives more access to the developers to make the decision whether they need to export the hidden Visio pages or not. The check of hiding the Visio pages is implemented for the output SVG, XPS, Image, HTML and PDF formats. This help topic shows how developers can include or exclude hidden pages of Visio in output files: Control the Export of Hidden Visio Pages on Saving

## Detect the Type of Visio File

Developers may come across the scenario to automate the identification of file type by its content. Using Aspose.Diagram API, they can now figure out how to distinguish the Visio file type before any other manipulation. Thus, they can also make groups of Visio files to execute in their applications. This help topic shows how developers can detect the Visio file format: Detect the Format of Visio File

## Improved Hebrew and Arabic Text Rendering

Aspose.Diagram API has provided support of reading and writing RTL (right to left) languages, such as Hebrew and Arabic. In this latest version, we have enhanced its export feature to place and render text in the same way as available in the input Visio diagram. We have fixed the problem of incorrect text direction as well as combining letters to form words in Arabic and Hebrew. We would really like to hear back from our users with their experiences in that area.

This new version also addresses the issues of losing textual style of the shapes, partial rendering of the text, missing shapes, wrong position of the shape and error messages while reading or writing diagrams. All this also improves the performance of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSD to PDF export - the table cell's text is partially invisible.
    
*   Fixed: VDX to PDF export - the text of various shapes is misplaced.
    
*   Fixed: VSD to SVG export is missing some Visio shapes.
    
*   Fixed: VSD to SVG export is not applying the inner white color of shapes.
    
*   Fixed: Open and save routine of VSDX has changed the text into dummy characters.
    
*   Fixed: Open and save routine of VSDX has changed the dotted line shaper.
    
*   Fixed: VSD to PDF export - the text items are misplaced.
    
*   Fixed: VSD to VDX export is throwing the Master element error.
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   FileFormatUtil and FileFormatInfo classes are added.
    
*   DetectFileFormat method is added to the FileFormatUtil Class.
    
*   FileFormatType property is added to the FileFormatInfo Class.
    
*   LoadFormat property is added to the FileFormatInfo Class.
    
*   ExportHiddenPage property is added in the SVGSaveOptions, XPSSaveOptions, ImageSaveOptions, HTMLSaveOptions and PdfSaveOptions classes.
    

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][2].
    
*   [Download Aspose.Diagram for .NET][3]
    
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
    
*   [Aspose.Diagram product family forum][4] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
    
*   [Enable email subscription][5] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
    
*   [Aspose.Diagram for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
    
*   Migrate from Earlier Versions of Aspose.Diagram API - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.
    

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.

# Edit a Page-Level Comment in the Visio




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: https://products.aspose.com/diagram
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposediagram/Aspose_diagram_NET




