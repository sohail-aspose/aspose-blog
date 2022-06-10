---
title: 'Show or Hide Visio Pages on Export using Java'
date: Tue, 10 May 2016 09:27:05 +0000
draft: false
url: /2016/05/10/show-or-hide-visio-pages-on-export-using-java/
author: Imran Rafique
summary: ''
tags: ['Convert Visio diagram', 'Hide Visio Page', 'Show Visio Page', 'Visio page visibility', 'master element', 'shape text']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce that the new version 6.3.0 of [Aspose.Diagram for Java][1] API is now live. The recent features give flexibility and control to the developers because we genuinely care about our clients and are dedicated to serving them well. Two features are incorporated with regular bug fixes and enhancements. Developers can show or hide pages of a Visio diagram in various output files like SVG, XPS, Image, HTML, and PDF. They can also identify the format of a Visio file by content. Let’s go into the details.

## Show or Hide the Pages of Visio Diagram while Exporting to SVG, XPS, Image, HTML and PDF

Using Aspose.Diagram API, developers were already able to hide or show the pages of any Visio diagram by setting the UIVisiblity cell in the page ShapeSheet. Developers may also require to export the Visio diagram in other supported file formats yet the export feature was not omitting the Visio pages with hidden visibility. It was including all the Visio pages in output files. This version adds ExportHiddenPage property in SVG, XPS, Image, HTML and PDF save options. The flexibility of this feature gives more control over the visibility of hidden Visio pages in the exported files. This help topic shows how developers can show or hide the pages of a Visio diagram: Control the Export of Hidden Visio Pages on Saving

## Identify the Format of Visio File

Identification of a Visio file format is crucial, as without that, developers may come across an error to open the file. Upon using Aspose.Diagram API, developers can now identify the file type by its content. Developers would also be able to sort Visio files by type to process identical files together with any application. This help topic shows how to identify the Visio file format: Detect the Format of Visio File

We have improved the ability of reading and writing VSDX diagrams using Aspose.Diagram API. Previously, it was changing the style of lines and text as well as rendering dummy characters. Another bug fix on exporting VDX, it was not rendering the grid lines of a Visio page in the output VSDX. Please check a list of the resolved defects:

*   Fixed: VDX to VSDX export marks the page grid line option checked.
*   Fixed: Open and save routine to VSDX has changed the text into dummy characters.
*   Fixed: Open and save routine to VSDX has changed the dotted line shape.
*   Fixed: Open and save routine of VSDX changes text font and boldness.
*   Fixed: VSD to VDX export is throwing the Master element error.

## Public API Changes

The following API changes in the new version are also worth noting:

*   FileFormatUtil and FileFormatInfo classes are added.
*   detectFileFormat method is added to the FileFormatUtil Class.
*   FileFormatType property is added to the FileFormatInfo Class.
*   LoadFormat property is added to the FileFormatInfo Class.
*   ExportHiddenPage property is added in the SVGSaveOptions, XPSSaveOptions, ImageSaveOptions, HTMLSaveOptions and PdfSaveOptions classes.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][2].
*   [Download Aspose.Diagram for Java][3].
*   [Aspose.Diagram for Java docs][4] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.

Intensity




[1]: https://products.aspose.com/diagram
[2]: https://products.aspose.com/diagram/net
[3]: https://downloads.aspose.com/diagram/net
[4]: https://docs.aspose.com/diagram/net
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposediagram/Aspose_Diagram_Java




