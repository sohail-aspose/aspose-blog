---
title: 'Support of Style Separator Enable or Disable Font Substitution Improved Importing Logic with KeepSourceFormatting and Metafile Rendering in HTML'
date: Tue, 13 Feb 2018 07:28:30 +0000
draft: false
url: /2018/02/13/aspose.words-for-.net-18.2/
author: Tahir Manzoor
summary: ''
tags: ['.NET Word API', 'Add style separator to Word documents in Csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.2][1]. This month’s release contains over 95 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   FontSettings.EnableFontSubstitution option added
*   Support to insert Style Separator to put different Paragraph styles
*   HtmlSaveOptions.MetafileFormat property added
*   KeepSourceFormatting logic improved
*   Rendering of SVG graphics elements embedded into DrawingML objects (svgBlip) implemented
*   Added option to disable the internal font substitution mechanism and use the default font instead while rendering to PDF. (FontSettings.EnableFontSubstitution)
*   Fixed "Compound lines are not supported" warning generation
*   Rendering of “DFKai-SB" TrueType font fixed
*   Fixed problem with path gradient brush scaling while rendering metafiles
*   Spacing between legend items in DrawingML Charts rendering fixed
*   The data series line with "Round" cap type is rendered properly when exporting DrawingML Charts into PDF now
*   Rotated VML text boxes with non-default alignment rendering fixed
*   Auto-size calculation of rotated VML text boxes with vertical layout fixed
*   Implemented none wrapping for text frames
*   Improved paragraph spacing computation with hidden paragraphs
*   Improved custom tab stops handling around hidden paragraphs
*   Improved line wrapping around dashes
*   Improved character spacing control for complex code point sequences
*   Improved processing of out-of-order footnotes
*   Implemented mirror margins and gutter position handling when page orientation changes
*   Improved performance of reflow when document is large and has fields in headers/footers
*   Fixed text box width issue with left-aligned RTL text

## Changed Importing Logic with KeepSourceFormatting Mode

In old versions of Aspose.Words, our import algorithm was different from what MS Word does. We imported style with expanded attributes. If a style already exists in the document, we applied a new name to it. MS Word does not import style if it already exists. It just expands attributes into the direct paragraph/run properties. We have improved the importing document logic with KeepSourceFormatting mode that is closer to MS Word's behavior. Now we are expanding source formatting into the direct attributes of imported nodes.

## Added Feature to Insert Style Separator to Put different Paragraph Styles

In this version of Aspose.Words, we have added the support of style separator to put different paragraph styles in the same printed paragraph. Style Separator can be added to the end of a paragraph using the Ctrl+Alt+Enter Keyboard Shortcut into MS Word. This feature allows for two different paragraph styles used in one logical printed paragraph. Please read following article for more detail.  
[Insert Style Separator to Put Different Paragraph Styles][4]

```
/// <summary>
/// Inserts style separator into the document.
/// </summary>
/// <remarks>
/// This method allows to apply different paragraph styles to two different parts of a text line.
/// </remarks>
public void InsertStyleSeparator() 
```

## Added Feature to Specify Metafile format When Exporting Document to HTML

In this version, we have added HtmlSaveOptions.MetafileFormat property to specify in what format metafiles are saved when exporting to HTML, MHTML, or EPUB. By default metafiles are rendered to raster PNG images. HtmlMetafileFormat enumeration has added to indicate the format in which metafiles are saved to HTML document. For more detail, please read following article.  
[Specify Metafile format When Exporting Document to HTML][5]

```
public class HtmlSaveOptions
{
    /// <summary>
    /// Specifies in what format metafiles are saved when exporting to HTML, MHTML, or EPUB.
    /// Default value is <see cref="HtmlMetafileFormat.Png" />, meaning that metafiles     /// are rendered to raster PNG images.
    /// </summary>
    /// <remarks>
    /// Metafiles are not natively displayed by HTML browsers.     /// By default, Aspose.Words converts WMF and EMF
    /// images into PNG files when exporting to HTML. Other options are to convert metafiles     /// to SVG images or to export
    /// them as is without conversion.
    /// Some image transforms, in particular image cropping, will not be applied to     /// metafile images if they are exported
    /// to HTML without conversion.
    /// </remarks>
    /// <seealso cref="ImageResolution"/>
    /// <seealso cref="ScaleImageToShapeSize"/>
    public HtmlMetafileFormat MetafileFormat
    {
        get { return mSaveImageOptions.MetafileFormat; }
        set { mSaveImageOptions.MetafileFormat = value; }
    }
}
 
/// <summary>
/// Indicates the format in which metafiles are saved to HTML documents.
/// </summary>
public enum HtmlMetafileFormat
{
    /// <summary>
    /// Metafiles are rendered to raster PNG images.
    /// </summary>
    Png,
    /// <summary>
    /// Metafiles are converted to vector SVG images.
    /// </summary>
    Svg,
    /// <summary>
    /// Metafiles are saved as is, without conversion.
    /// </summary>
    EmfOrWmf
}
```

This new property replaces HtmlSaveOptions.ExportMetafileAsRaster which is now marked obsolete. The new code should use MetafileFormat instead of ExportMetafileAsRaster, as shown below:

```
MetafileFormat = HtmlMetafileFormat.Png;
// Instead of
ExportMetafileAsRaster = true;
 
MetafileFormat = HtmlMetafileFormat.EmfOrWmf;
// Instead of
ExportMetafileAsRaster = false;
```

## Added Feature to Enable/Disable Font Substitution

We have added new property FontSettings.EnableFontSubstitution in this version of Aspose.Words to specify whether to enable or disable font substitution. Please read following article for more detail.  
[Enable or Disable Font Substitution][6]

```
 /// <summary>
/// Specifies whether to enable or disable font substitution.
/// </summary>
/// <remarks>
/// <para>If font substitution is enabled, Aspose.Words evaluates all the related fields in <see cref="FontInfo"/>
/// (Panose, Sig etc) for the missing font and finds the closest match among the available font sources. Note that
/// font substitution mechanism will override the <see cref="DefaultFontName"/> in cases when <see cref="FontInfo"/>
/// for the missing font is available in the document.</para>
/// <para>If font substitution is disabled, Aspose.Words uses the <see cref="DefaultFontName"/> for the substitution
/// of missing fonts.</para>
/// <para>The default value is <c>true</c>.</para>
/// </remarks>
public bool EnableFontSubstitution
{
    get; set;
}
```

## Obsolete Properties were Removed from Aspose.Words API

*   The **HtmlSaveOptions.AllowNegativeLeftIndent** has removed. Please use HtmlSaveOptions.AllowNegativeIndent property.
*   The **HtmlSaveOptions.ExportHeadersFooters** has removed. Please use HtmlSaveOptions.ExportHeadersFootersMode property.
*   The **HtmlFixedSaveOptions.MetafileRenderingMode** has removed. Please use the HtmlFixedSaveOptions.MetafileRenderingOptions.RenderingMode property.
*   The **SvgSaveOptions.MetafileRenderingMode** has removed. Please use the SvgSaveOptions.MetafileRenderingOptions.RenderingMode property.
*   The **XpsSaveOptions.HeadingsOutlineLevels** was removed. Please use OutlineOptions.HeadingsOutlineLevels property.
*   The **XpsSaveOptions.BookmarksOutlineLevel** was removed. Please use OutlineOptions.DefaultBookmarksOutlineLevel property.
*   The **XpsSaveOptions.MetafileRenderingMode** was removed. Please use MetafileRenderingOptions.RenderingMode property.

## Obsolete SWF File Format was Removed from Aspose.Words API

Adobe is going to drop support of Flash that is why we decided to remove SaveFormat.Swf from Aspose.Words API. The SaveFormat.Swf has removed.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][7].
2.  [Install using NuGet Package][8]
3.  [Documentation][9] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
6.  [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.2+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Working+with+Styles#WorkingwithStyles-InsertStyleSeparatortoPutDifferentParagraphStyles
[5]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-SpecifyMetafileformatWhenExportingDocumenttoHTML
[6]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-EnableorDisableFontSubstitution
[7]: https://products.aspose.com/words/net
[8]: https://www.nuget.org/packages/Aspose.Words/
[9]: https://docs.aspose.com/display/wordsnet
[10]: https://apireference.aspose.com/net/words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




