---
title: 'Basic API to Manipulate Themes Added, Improved Footnote Balancing, PDF Background Rendering and Many other Improvements Added in Aspose.Words 15.7.0'
date: Tue, 11 Aug 2015 16:33:08 +0000
draft: false
url: /2015/08/11/basic-api-to-manipulate-themes-added-improved-footnote-balancing-pdf-background-rendering-and-many-other-improvements-added-in-aspose.words-15.7.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 15.7.0 has been released. This month’s release contains over 115 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.7.0][1]
*   [Aspose.Words for Java 15.7.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Added API to work with Themes
*   Allow inserting of TIFF images
*   API to change footnote/endnote separator
*   Improved footnote balancing
*   Improved text wrapping around objects in footers
*   Ternary raster operations for EMF/WMF rendering implemented
*   PDF background rendering improved
*   Text with gradient fill rendering implemented
*   Japanese OTF fonts overlapping characters problem in rendered images fixed

## Basic API to Programmatically Manipulate Themes Added

WORDSNET-10513 is now resolved. We have added basic API to access document theme properties. Please refer to the following article: How to Manipulate Theme Properties

## Font.AutoColor Property Added

WORDSNET-2768 is now resolved. Aspose.Words now can determine actual color of text output that will be used for the "auto color" using the following property:

```
 public Color AutoColor; 
```

It returns the present calculated color of the text (black or white) to be used for 'auto color'. If the color is not 'auto' then it returns Color.

When text has 'automatic color', the actual color of text is calculated automatically so that it is readable against the background color. As you change the background color, the text color will automatically switch to black or white in MS Word to maximize legibility.

Usage example is as follows:```
 Run run = new Run(new Document());
run.Font.Color = Color.Empty; // Remove direct color, so it can be calculated automatically with Font.AutoColor.
            
run.Font.Shading.BackgroundPatternColor = Color.Black; // Set dark background for the text.
Console.WriteLine(run.Font.AutoColor); // returns Color.White.

run.Font.Shading.BackgroundPatternColor = Color.White; // Set light background for the text.
Console.WriteLine(run.Font.AutoColor); // returns Color.Black. 
```

## TextOrientation.VerticalRotatedFarEast Option Added

WORDSNET-12039 is now implemented and the following property added to the API:

```
 public TextOrientation.VerticalRotatedFarEast = 7; 
```

It specifies orientation of text on a page, in a table cell or a text frame as following: Far East characters appear vertical, other text is rotated 90 degrees to the right to appears from top to bottom vertically, then left to right horizontally (tb-lr-v). Use-case is as follows:

```
 Document doc = new Document("path to document");
Cell cell = (Cell) doc.GetChild(NodeType.Cell, 0, true);
 
// Set text orientation for Far East characters appear vertical, other text is rotated 90 degrees to the right to appears from top to bottom vertically, then left to right horizontally.
cell.CellFormat.Orientation = TextOrientation.VerticalRotatedFarEast; 
```

## SaveOptions.UpdateSdtContent is added

WORDSNET-12111 is now resolved. This option controls whether content of StructuredDocumentTag is updated before document saving. Default value is TRUE.

```
 Document doc = new Document("c:\test.docx");
 
SaveOptions so = SaveOptions.CreateSaveOptions(SaveFormat.Docx);            
so.UpdateSdtContent = false;
 
doc.Save("C:\test.pdf", so);            // SDT content will not be updated and rendered as is. 
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx




