---
title: 'Encrypt OpenDocument and Preserve PaperTray Information in PCL using C#'
date: Mon, 09 Apr 2018 16:43:07 +0000
draft: false
url: /2018/04/09/encrypt-opendocument-ans-preserve-papertray-information-in-pcl-using-csharp/
author: Tahir Manzoor
summary: ''
tags: ['Encrypt OpenDocument using Csharp', 'Preserve PaperTray Information in PCL']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.4][1]. This month’s release contains over 66 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Provide an ability to work with password-protected ODT and OTT file formats
*   Preserve PaperTray information in PCL
*   Added ShapeBase.IsLayoutInCell property
*   Implemented optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MS Word when saving metafiles as vector graphics to PDF, XPS, etc.
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

## Work with Password-Protected ODT and OTT File Formats

In this version of Aspose.Words, we have added support to export document to ODT and OTT files encrypted with a password. Please read the following article for more detail.

*   [Open and Save Encrypted OpenDocument][4]

The following public API has been added to the OdtSaveOptions class:

```
/// <summary>
/// Initializes a new instance of this class that can be used to save a document in /// the <see cref="Words.SaveFormat.Odt"/> format encrypted with a password.
/// </summary>
public OdtSaveOptions(string password)
```
```
/// <summary>
/// Gets or sets a password to encrypt document.
/// </summary>
/// <remarks>
/// <para>In order to save document without encryption this property should be null /// or empty string.</para>
/// </remarks>
public string Password
```

## Preserve PaperTray Information in PCL

We have added support to preserve paper tray information when exporting document to PCL format. No additional code is required. Following information is transferred from document's model to PCL file.

```
PageSetup.FirstPageTray
PageSetup.OtherPagesTray
```

Please note that the value of paper tray is passed from document as is. PCL format supports only 8-bit identifiers for paper tray so make sure this values are correct for PCL printer.

## Added ShapeBase.IsLayoutInCell property

We have added ShapeBase.IsLayoutInCell property in this version of Aspose.Words. This property gets or sets a flag indicating whether the shape is displayed inside a table or outside of it. The property may be helpful for shapes (mainly VML) that are placed into a table cell but are needed to position without binding to the cell. Please refer to the following article.

*   [How to Add a Watermark in Table Cell][5]

```
/// <summary>
/// Gets or sets a flag indicating whether the shape is displayed inside a table or outside of it.
/// </summary>
/// <remarks>
/// The default value is <b>true</b>.
/// Has effect only for top level shapes, the property <see cref="WrapType"/> of which is set to value
/// other than <see cref="WrapType.Inline"/>.
/// </remarks>
public bool IsLayoutInCell
{
    get; set;
}
```

## Optimization of Vector Graphics Output of Metafile Rendering

We have implemented the optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MS Word when saving metafiles as vector graphics to PDF, XPS, etc.

Optimization may affect the visual appearance of metafile vector graphics in viewer applications due to the peculiarities of vector graphics rendering. For example, there are cases when not optimized output looks faded out in Acrobat Reader comparing to optimized output.

Metafile output optimization is controlled by existing FixedPageSaveOptions.OptimizeOutput flag.

## Obsolete property LoadOptions.WebRequestTimeout was removed

We have removed obsolete property WebRequestTimeout from the LoadOptions class in Aspose.Words 18.4. Please use the HtmlLoadOptions.WebRequestTimeout property instead.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][6].
2.  [Install using NuGet Package][7]
3.  [Documentation][8] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][9] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][10]
    *   [Paid Support Forum][11]
6.  [Enable Blog Subscription][12] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.4+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-OpenandSaveEncryptedOpenDocument
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Watermark#WorkingwithWatermark-HowtoAddaWatermarkinTableCell
[6]: https://products.aspose.com/words/net
[7]: https://www.nuget.org/packages/Aspose.Words/
[8]: https://docs.aspose.com/display/wordsnet
[9]: https://apireference.aspose.com/net/words
[10]: https://forum.aspose.com/c/words
[11]: https://helpdesk.aspose.com/
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-.NET




