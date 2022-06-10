---
title: 'Work with Password Protected ODT or OTT File and Preserve PaperTray Information in PCL using Aspose.Words for Java 18.4'
date: Fri, 13 Apr 2018 04:19:45 +0000
draft: false
url: /2018/04/13/aspose.words-for-java-18.4-released/
author: Awais Hafeez
summary: ''
tags: ['Preserve PaperTray in PCL in Java', 'Work with password protected ODT or OTT in Java']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.4**][1]. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.4][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Public Ref Class for out-ref Emulation Added in Java API

Related issue: WORDSJAVA-1756  
On .NET baseline, some public API methods contain out/ref params in signatures. Service classes Ref, RefInt, RefBoolean, etc. are added to emulate out/ref in Java. Now, the code like:

```
void SomeMethod(ref Document doc, out int i)
```

It is autoported to Aspose.Words for Java as:

```
void someMethod(Ref doc, RefInt i)
```

The Ref\* classes contain get() and set() methods to get and set the value.

## Ability to Work with Password-Protected ODT and OTT File Formats

The OdtSaveOptions class can be used to specify additional options when saving a document into the ODT or OTT format. You can initializes a new instance of this class that can be used to save a document in the ODT format encrypted with a password. You can also use OdtSaveOptions.Password property to get or set password to encrypt document. The code sample below shows how to load and save OpenDocument encrypted with password.  
[Open and Save Encrypted OpenDocument][3]

## Ability to Preserve PaperTray Information in PCL Added

We have added support to preserve paper tray information when exporting document to PCL format. No additional code is required. Following information is transferred from document's model to PCL file.

```
PageSetup.FirstPageTray
PageSetup.OtherPagesTray
```

Please note that the value of paper tray is passed from document as is. PCL format supports only 8-bit identifiers for paper tray so make sure this values are correct for PCL printer.

## ShapeBase.IsLayoutInCell Property Added

We have added ShapeBase.IsLayoutInCell property in this version of Aspose.Words. This property gets or sets a flag indicating whether the shape is displayed inside a table or outside of it. The property may be helpful for shapes (mainly VML) that are placed into a table cell but are needed to position without binding to the cell. Please refer to the following article.  
[How to Add a Watermark in Table Cell][4]

## Optimization of Vector Graphics Output of Metafile Rendering

We have implemented the optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MS Word when saving metafiles as vector graphics to PDF, XPS, etc. Optimization may affect the visual appearance of metafile vector graphics in viewer applications due to the peculiarities of vector graphics rendering. For example, there are cases when not optimized output looks faded out in Acrobat Reader comparing to optimized output. Metafile output optimization is controlled by existing FixedPageSaveOptions.OptimizeOutput flag.

## Obsolete LoadOptions.WebRequestTimeout Property Removed

We have removed obsolete property WebRequestTimeout from the LoadOptions class in Aspose.Words 18.4. Please use the HtmlLoadOptions.WebRequestTimeout property instead.

## Other Improvements

There are 75 improvements and fixes in this regular monthly release. The most notable are:

*   Added public Ref<T> class for out/ref emulation in public API.
*   Provide an ability to work with password-protected ODT and OTT file formats
*   Preserve PaperTray information in PCL    
*   Added ShapeBase.IsLayoutInCell property 
*   Implemented optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MW when saving metafiles as vector graphics to PDF, XPS, etc.
*   PaperTray information is now saved in PCL output
*   "DrawingML shapes are not fully supported" warning is not thrown anymore, more specific warnings are used instead while rendering
*   DrawingML shapes with auto-size and empty textboxes don't throw exception while rendering now
*   WordArt objects with empty fill now cast only outline shadows while rendering. Previously the whole shape cast a shadow
*   Improved rendering of MathAccentElement. The accent symbol is rendered in accordance with the letter's height
*   Improved rendering of PieChart, if data labels have a manual layout
*   Improved rendering of the text boxes with OleObjects (e.g. Math equation)
*   Improved rendering of WordArt objects with gradient fill
*   Fixed a bug causing the corruption of radial gradient fill for rotated shapes while rendering
*   Fixed rendering of “Monotype Hadassah” font with legacy encoding
*   Fixed a problem with META\_SETPIXEL WMF record while rendering meta-files
*   Improved frame width calculation when paragraph has right indent
*   Improved computation of widths of ideographic space when combined with document grid, space inside footnotes
*   Improved floating table positioning for RTL tables in 2013 compatibility mode
*   Improved layout of 2013 compatible documents when page break overlaps footer
*   Improved positioning of wrapped lines in 2013 compatibility mode, and lines with large inline images
*   Fixed issue with character compressing when Kinsoku rule is ignored by document
*   Fixed incorrect glyph selection for Zero Width No-Break Space when font does not have this glyph
*   Fixed comment range highlighting issue when comment spans multiple pages inside a repeated header row of a table
*   Fixed rendering of text in merged cells when row contains hidemark attribute on the cell break and all remaining cells are merged

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][5]
*   [Install Aspose.Words for Java from Maven][6]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][7]
    *   [Paid Support Forum][8]
*   [Aspose.Words for Java online documentation][9]– Help documentation.
*   [Aspose.Words for Java online API reference][10]– API reference documents.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][12] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.4+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-OpenandSaveEncryptedOpenDocument
[4]: https://docs.aspose.com/display/wordsjava/Working+with+Watermark#WorkingwithWatermark-HowtoAddaWatermarkinTableCell
[5]: https://products.aspose.com/words/java
[6]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[7]: https://forum.aspose.com/c/words
[8]: https://helpdesk.aspose.com/
[9]: https://docs.aspose.com/display/wordsjava/Home
[10]: https://apireference.aspose.com/java/words
[11]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[12]: https://github.com/aspose-words/Aspose.Words-for-Java




