---
title: 'Control Images when Rendering Excel Files as HTML using Java'
date: Tue, 20 May 2014 08:26:07 +0000
draft: false
url: /2014/05/20/control-the-images-while-rendering-spreadsheets-to-html/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells', 'Aspose.Cells for Java', 'Babar Raza', 'Excel Comments', 'Excel Java Component', 'Excel files to HTML', 'HTML to Excel files', 'HtmlLoadOptions', 'HtmlSaveOptions', 'Image Resolution in HTML files', 'Image Type', 'Interpret formulas', 'RenderingHints', 'Text Direction']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We have our regular monthly [Aspose.Cells for Java][1] release ready for you to [download][2]. Before you start exploring the new added features & enhancement, here is a look at just a few of the biggest features in this month’s release.

For a full list of bug fixes and improvements please refer to the release notes in the above link.

## Set the Direction of Text in Shapes

Aspose.Cells for Java 8.0.2 has provided the getter & setter for the TextDirection property in the Shape class. The aforesaid property now lets developers to control the direction of the text in shapes including the spreadsheet comments. The setTextDirection method accepts a value from the constants TextDirectionType, and applies the text direction as one of the following:

*   Left to Right
*   Right to Left
*   Context

## Control the Images while Rendering Spreadsheets to HTML

Prior to this release, developers couldn't control images when exporting spreadsheets (Excel files) to HTML format. Starting with Aspose.Cells for Java 8.0.2, the API has exposed the ImageOptions for the HtmlSaveOptions class, allowing developers to set preferences for images in output HTML files. ImageOptions has brought a great deal of features that can be set. A few of the most important settings are listed below.

*   The image format can be set.
*   The image quality can be specified from a range of 0 to 100 if ImageFormat is set to Jpeg.
*   The compression type can be set when the ImageFormat is set to Tiff.
*   The background transparency can be set if the specified ImageFormat is set to Png.
*   Rendering hints allow specifying smoothing edges to the text as well as lines and curves.
*   Vertical & horizontal resolution of the images.

## Enhancements to the HtmlLoadOptions Class

Another notable enhancement has been made to the HtmlLoadOptions class by exposing the Boolean ConvertFormulasData property. Setting this property to true when using the setConvertFormulasData method allows the API to interpret any string value starting with character “=” as a formula.

This is how you can use the property.

```
//Create an instance of HTMLLoadOptions
HTMLLoadOptions load = new HTMLLoadOptions();

//Set ConvertFormulasData to true
load.setConvertFormulasData(true);

//Load a spreadsheet to be converted
Workbook book = new Workbook(myDir + "chart.html", load); 
```

Please note the default value of ConvertFormulasData is false.

## Bug Fixes

Aspose.Cells for Java 8.0.2 has provided fixes for several important issues, such as a couple of problems related to rendering PivotTables as PDF, range references, deleting columns & AutoFitRows with different font settings.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Cells support forum][3] for a chat.




[1]: https://products.aspose.com/cells/java
[2]: https://downloads.aspose.com/cells/java
[3]: https://forum.aspose.com/




