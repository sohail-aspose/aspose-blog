---
title: 'Render Images in CMYK Color Space in Word to PDF in C# and Java'
date: Sun, 10 Aug 2014 05:38:46 +0000
draft: false
url: /2014/08/10/render-images-in-cmyk-color-space-in-word-to-pdf-in-csharp-java/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 14.7.0 has been released with this month’s release containing over 114 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.7.0][1]
*   [Aspose.Words for Java 14.7.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improvements to DrawingML shadow, extrusion, and 3D rendering algorithms
*   New public API to specify revision marks appearance for rendering
*   Vertical text is supported in HTML, MHTML, and EPUB
*   Improvements to rendering and line wrapping for Arabic and the Far East scripts
*   Improvements to the rendering of inline shapes within the rotated text

## ImageColorSpaceExportMode Property Added to PdfSaveOptions Class

Images in PDF documents now can be saved in CMYK color space. It is controlled by PdfSaveOptions.ImageColorSpaceExportMode property.

```
/// <summary>
/// Specifies how the color space will be selected for the images in PDF document.
/// </summary>
/// <remarks>
/// The default value is <see cref="PdfImageColorSpaceExportMode.Auto"/>.
/// If <see cref="PdfImageColorSpaceExportMode.SimpleCmyk"/> value is specified,
/// <see cref="ImageCompression"/> option is ignored and
/// Flate compression is used for all images in the document.
/// </remarks>
public PdfImageColorSpaceExportMode ImageColorSpaceExportMode {get;set;}
```

Where PdfImageColorSpaceExportMode is a newly introduced enumeration:

```
/// <summary>
/// Specifies how the color space will be selected for the images in PDF document.
/// </summary>
public enum PdfImageColorSpaceExportMode
{
/// <summary>
/// Aspose.Words automatically selects the most appropriate color space for each image.
/// </summary>
/// <remarks>
/// <para>Most of the images are saved in RGB color space. Also Indexed and Grayscale color spaces may be used. CMYK color space is never used.</para>
/// <para>For some images the color space may be different on different platforms.</para>
/// </remarks>
Auto,
/// <summary>
/// Aspose.Words coverts RGB images to CMYK color space using simple formula.
/// </summary>
/// <remarks>
/// <para>
/// Images in RGB color space are converted to CMYK using formula:
/// Black   = minimum(1-Red,1-Green,1-Blue).
/// Cyan    = (1-Red-Black)/(1-Black).
/// Magenta = (1-Green-Black)/(1-Black).
/// Yellow  = (1-Blue-Black)/(1-Black).
/// RGB values are normalized - they are between 0 and 1.0.
/// </para>
/// </remarks>
SimpleCmyk
}
```

If the user wants to save images in PDF in CMYK color space, he can achieve this by using the following code:

```
PdfSaveOptions options = new PdfSaveOptions();
// Set CMYK color space for images in the PDF document.
options.ImageColorSpaceExportMode = PdfImageColorSpaceExportMode.SimpleCmyk;
doc.Save("MyDocument.pdf", options);
```

Note that the current implementation of CMYK support has some restrictions: JPEG codec is not supported; simple formula for RGB to CMYK conversion is used, no ICC profiles are supported.

## Priority Property Added to FontSourceBase Class

Priority property has been added to the FontSourceBase class. This property is used when there are fonts with the same family name and style in different font sources. In this case Aspose.Words selects the font from the source with the higher priority value. Please use the following code to achieve this:

```
// Aspose.Words will prefer fonts from "Folder1" over the fonts from "Folder2".
FolderFontSource folder1 = new FolderFontSource("Folder1", false, 2);
FolderFontSource folder2 = new FolderFontSource("Folder2", false, 1);
FontSettings.SetFontsSources(new FontSourceBase[] {folder1, folder2});
```

## ShowRevisionMarks, ShowRevisionBars and ShowOriginalRevision Added to Document.LayoutOptions.RevisionOptions Class

The following three new public members are added to the Document.LayoutOptions.RevisionOptions class:

```
/// <summary>
/// Allow to specify whether revision text should be marked with special formatting markup.
/// Default value for this property is <c>true</c>.
/// </summary>
public bool ShowRevisionMarks {get;set;}
 
/// <summary>
/// Allows to specify whether revision bars should be rendered near lines containing revised content.
/// Default value for this property is <c>true</c>.
/// </summary>
public bool ShowRevisionBars {get;set;}
 
/// <summary>
/// Allows to specify whether the original text should be shown instead of revised one.
/// Default value for this property is <c>false</c>.
/// </summary>
public bool ShowOriginalRevision {get;set;}
```

## New Public Values Added for ParagraphAlignment Enumeration

The following new public values are added to the ParagraphAlignment enumeration:

```
/// <summary>
/// Arabic only. Kashida length for text is extended to a medium length determined by the consumer.
/// </summary>
ArabicMediumKashida = 5,
 
/// <summary>
/// Arabic only. Kashida length for text is extended to its widest possible length.
/// </summary>
ArabicHighKashida = 7,
 
/// <summary>
/// Arabic only. Kashida length for text is extended to a slightly longer length.
/// </summary>
ArabicLowKashida = 8,
 
/// <summary>
/// Thai only. Text is justified with an optimization for Thai.
/// </summary>
ThaiDistributed = 9
```




[1]: http://downloads.aspose.com/words/net
[2]: http://downloads.aspose.com/words/java




