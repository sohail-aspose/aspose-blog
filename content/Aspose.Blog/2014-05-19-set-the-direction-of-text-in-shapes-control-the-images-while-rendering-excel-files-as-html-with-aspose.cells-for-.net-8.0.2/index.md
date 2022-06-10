---
title: 'Set the Direction of Text in Shapes &amp; Control the Images while Rendering Excel Files as HTML with Aspose.Cells for .NET 8.0.2'
date: Mon, 19 May 2014 18:44:51 +0000
draft: false
url: /2014/05/19/set-the-direction-of-text-in-shapes-control-the-images-while-rendering-excel-files-as-html-with-aspose.cells-for-.net-8.0.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png)Aspose.Cells for .NET 8.0.2 has been released. The new release contains a number of new features and enhancements.  It also includes several new fixes and other improvements. Moreover, we have fixed some bugs in the web based Grid control provided by Aspose.Cells for .NET for loading and manipulating Microsoft Excel files and calculating spreadsheet formulas. Before you go ahead and start exploring the new features & enhancement, we will list a few of the biggest features in this month’s release.

## Set the Direction of Text in Shapes

Aspose.Cells for .NET 8.0.2 provides the TextDirection property in the Shape class. The attribute now allows developers to control the direction of the text in shapes including spreadsheet comments. The property accepts a value from the constants TextDirectionType, and applies the text direction as one of the following:

*   Left to Right
*   Right to Right
*   Context

Please see the document on how to change the text direction of a comment for your reference.

## Control the Images when Rendering Spreadsheets to HTML

Before this release, developers couldn't control images when exporting spreadsheets (Microsoft Excel files) to HTML format. With the release of Aspose.Cells for .NET 8.0.2, the API has exposed the ImageOptions method for the HtmlSaveOptions class, allowing developers to set preferences for the images in the output HTML files. ImageOptions has brought a great deal of features that can be set. A few of the most important settings are listed below:

*   The image format can be set.
*   The image quality can be specified from a range of 0 to 100 if ImageFormat is set to Jpeg.
*   The compression type can be set when the ImageFormat is set to Tiff.
*   The background transparency can be set if the specified ImageFormat value is set to Png.
*   Rendering hints allows you to specify the smoothing edges to the text as well as lines and curves.
*   Vertical & horizontal resolution of images

Please see the document on how to set image preferences for the output HTML.

## Enhancements to the HtmlLoadOptions Class

Another significant enhancement has been made to the HtmlLoadOptions class by exposing the Boolean ConvertFormulasData property. Setting this property to true allows the API to interpret any string value starting with the character “=” as a formula

## Other Enhancements and Fixes

In the new version, we have fixed a few exceptions that occurred when reading Microsoft Excel files, manipulating advanced conditional formatting and converting Excel files to PDF format.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, applying style and formatting, rendering and manipulating pivot tables, manipulating shapes, rendering images from Excel worksheets, Smart Markers, applying auto-fit rows and columns, adding page breaks, header and footers, rendering and manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. A few enhancements have also been made to Aspose.Cells for .NET's formula calculation engine.

We also fixed a few bugs in the web based Grid control provided by Aspose.Cells for .NET regarding rendering shapes and table/list objects, numbers formatting, context menu and formula calculations, etc.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.0.2, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry545705.aspx




