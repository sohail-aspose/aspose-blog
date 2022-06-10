---
title: 'Convert Word to SVG and Set Default Font with Enhanced Fonts Selection Interface in Aspose.Words 11.1.0'
date: Thu, 01 Mar 2012 12:50:11 +0000
draft: false
url: /2012/03/01/new-svg-save-format-default-font-option-and-enhanced-fonts-selection-interface-in-aspose.words-11.1.0/
author: Adam Skelton
summary: ''
tags: ['Convert DOC to SVG', 'Convert DOCX to SVG', 'Convert Word to SVG']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We are proud to announce the latest release of Aspose.Words 11.1.0. This month’s release provides a brand new save format, you can now export any document loaded into Aspose.Words to the SVG vector image format.

We regularly produce a new release at the end of each month and this month’s release contains 102 various features and fixes.

As usual, you can download Aspose.Words from:

*   [Aspose.Words for .NET 11.1.0][1]
*   [Aspose.Words for Java 11.1.0][2]

Let’s take a look at a few of the prominent features included in the Aspose.Words 11.1.0 release:

## Save as the SVG Vector Image Format



{{< figure align=center src="images/SvgFormatLogo.jpg" alt="Save Word as SVG">}}


We now provide the export of any document to SVG format. This adds to the collection of image formats you can already save a document to using Aspose.Words. These include the raster types BMP, JPG, PNG, TIFF and the vector format EMF.

The code to achieve the conversion is simple, one line to load the document into Aspose.Words, the other to save it to SVG at the desired location.

```
Document doc = new Document("Rendering.doc");
doc.Save("Rendering Out.svg");
```

This format is newly introduced but it is already supported with high fidelity. Just take a look at the sample conversion below.

The first is the input Word document as seen in Microsoft Word, as you can see it contains plenty of formatting and different features.

Now the output produced by Aspose.Words converting the document to SVG image format. The output is viewed in Chrome. Clipping of the bottom border does not appear in the source image.



{{< figure align=center src="images/SvgOutputPage1.jpg" alt="">}}




{{< figure align=center src="images/SvgOutputPage2.jpg" alt="">}}


Also, here is a part of the source of the SVG image above produced by Aspose.Words. You can see the SVG markup of the image:



{{< figure align=center src="images/SvgSourceScreen-1024x535.jpg" alt="">}}


Lastly, we have introduced a new save options class to along with this save format. The **SvgSaveOptions** class provides you further control over how the SVG files are produced. A few of the features included in these save options are:

*   Saving images embedded into the SVG as base64 format.
*   Selecting how text is exported, you can choose to embed the text as static glyphs, use SVG fonts, or rely on the fonts of the target machine.
*   The selected page range of the document to save to image.

## Specify the Default Font used during Rendering

In previous versions, during rendering, if a required font was not found on the machine or embedded in the document then in most cases Aspose.Words would fall back on the free _“Gentium”_ font. Now, starting with this release you can specify the default to use during rendering if a font is missing.

Simply use the **DefaultFontName** property before rendering to set the default font:

```
FontSettings.DefaultFontName = "Arial";
```

## Different Options for Passing Fonts to Aspose.Words

It’s understandable that each user has their requirements when it comes to specifying where fonts come from. Not all users store their fonts on disk, however, Aspose.Words needs access to them one way or another to render documents correctly. We have listened to your requests on this subject and to help solve this issue have provided a brand new interface to make passing fonts to Aspose.Words even easier.

Now, you can pass any TrueType fonts to the Aspose.Words engine in a variety of different ways:

*   Using the **FileFontSource** class to load a font from the file.
*   Using the **MemoryFontSource** to pass a font in from an array of bytes.
*   Using **FolderFontSource** to load fonts from a folder or subfolders.

Here’s a quick example of this code in action:

```
// Create font sources from different locations.
FileFontSource fileFont = new FileFontSource(MyDir + "apr11.ttf");
MemoryFontSource memoryFont = new MemoryFontSource(GetFontBytes());
FolderFontSource folderFonts = new FolderFontSource("C:\\MyFonts\\", true);

// Pass these fonts to Aspose.Words
FontSettings.SetFontsSources(new FontSourceBase[] {fileFont, memoryFont, folderFonts});
```

As before all of the existing functionality still exists, you can still set font folders using the existing **SetFontFolder** method. Additionally Aspose.Words still searches for fonts in the expected font locations, such as _“C:\\Windows\\Fonts\\”_ on a Windows machine.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




