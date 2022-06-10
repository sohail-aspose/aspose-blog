---
title: 'Support for Shape Connectors, Improvements in Tight Wrapping, Overlapped and Nested Floating Objects and many New Members Added in Aspose.Words 14.12.0'
date: Wed, 14 Jan 2015 10:08:16 +0000
draft: false
url: /2015/01/14/support-for-shape-connectors-improvements-in-tight-wrapping-overlapped-and-nested-floating-objects-and-many-new-members-added-in-aspose.words-14.12.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 14.12.0 has been released. This month’s release contains over 103 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.12.0][1]
*   [Aspose.Words for Java 14.12.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   WordArt rendering does not rely on GDI+ now and supported on .NET, Mono and Java
*   New mode of handling styles during Import via public ImportFormatMode.KeepDifferentStyles
*   Public API for specifying text effects for Revisions during rendering to fixed formats
*   Shape connectors supported
*   Improved tight wrapping mode for floating objects
*   Improved rendering of overlapped and nested floating objects
*   Enhanced inter-characters spacing calculation for Asian documents with kerning
*   Improved text direction detection for documents with missing RTL attributes
*   Hyperlinks on shapes and text inside textboxes are exported correctly to HTML

## New Mode of Handling Styles during Import via Public ImportFormatMode.KeepDifferentStyles

We have introduced a new KeepDifferentStyles option in ImportFormatMode which can be used to only copy styles that are different from those in the source document. This option allows to reuse destination styles if the formatting they provide is identical to the styles in the source document. If the style in destination document is different from the source then it is imported. Please see the following code for an example usage

```
 Document dst = new Document("src.docx"); 
Document src = new Document("dst.docx");
 
// Upon appending with KeepDifferentStyles, only styles that have differences in formatting (as compared to their identically named counterparts in the source doc) will be copied to the destination document. 
dst.AppendDocument(src, ImportFormatMode.KeepDifferentStyles);
 
dst.Save("out.docx"); 
```

## Saving to OpenDocument (ODT) Version 1.2 Supported

For output ODT documents, Aspose.Words now supports the following OpenDocument versions:

*   'office:version = "1.1"' is specified when ' OdtSaveOptions.IsStrictSchema11 = true'
*   'office:version = "1.2"' is specified when ' OdtSaveOptions.IsStrictSchema11 = false'

## PageHorizontalAlignment and PageMargins Properties Added to HtmlFixedSaveOptions Class

The following properties are added to the public API

```
 /// <summary>
/// Specifies the horizontal alignment of pages in an HTML document.
/// Default value is <c>HtmlFixedHorizontalPageAlignment.Center</c>.
/// </summary>
public HtmlFixedPageHorizontalAlignment PageHorizontalAlignment
{
    get { return mPageHorizontalAlignment; }
    set { mPageHorizontalAlignment = value; }
} 
```
```
 /// <summary>
/// Specifies the horizontal alignment for pages in output HTML document.
/// </summary>
public enum HtmlFixedPageHorizontalAlignment
{
    /// <summary>
    /// Align pages to the left.
    /// </summary>
    Left,
 
    /// <summary>
    /// Center pages. This is the default value.
    /// </summary>
    Center,
 
    /// <summary>
    /// Align pages to the right.
    /// </summary>
    Right
} 
```
```
 /// <summary>
/// Specifies the margins around pages in an HTML document.
/// The margins value is measured in points and should be equal to or greater than 0.
/// Default value is 10 points.
/// </summary>
/// <remarks>
/// <para>Depends on the value of <see cref="PageHorizontalAlignment"/> property:</para>
/// <list type="bullet">
/// <item>
/// Defines top, bottom and left page margins if the value is <see cref="HtmlFixedPageHorizontalAlignment.Left"/>.
/// </item>
/// <item>
/// Defines top, bottom and right page margins if the value is <see cref="HtmlFixedPageHorizontalAlignment.Right"/>.
/// </item>
/// <item>
/// Defines top and bottom page margins if the value is <see cref="HtmlFixedPageHorizontalAlignment.Center"/>.
/// </item>
/// </list>
/// </remarks>>
public double PageMargins
{
    get { return mPageMargins; }
    set
    {
        if (value < 0)
            throw new ArgumentException("value");
        mPageMargins = value;
    }
} 
```

To remove the margin declaration, set PageHorizontalAlignment to HtmlFixedPageHorizontalAlignment.Left and PageMargins to 0.

## AllowTrailingWhitespaceForListItems Property Added to LoadOptions Class

This flag allows to specify how numbered list items are recognized when document is imported from plain text format. The default value is true. This property is used only when loading plain text documents. If set to true, lists recognition algorithm allows list numbers to end with either dot or whitespace character. If this option is set to false then the list item is only recognized as such if the leading number is ending with dot "." symbol.

```
 public bool AllowTrailingWhitespaceForListItems
{
    get { return mAllowTrailingWhitespaceForListItems; }
    set { mAllowTrailingWhitespaceForListItems = value; }
} 
```

## Public API for Specifying Text Effects for Revisions during Rendering to Fixed Page Formats

The following public entities exposed:

```
 /// <summary>
/// Allows to specify decoration effect for revisions of document text.
/// </summary>
public enum RevisionTextEffect 
```

The following public properties with getters/setters added to RevisionOptions class:

```
 public RevisionTextEffect InsertedTextEffect

public RevisionTextEffect DeletedTextEffect

public RevisionTextEffect MovedFromTextEffect

public RevisionTextEffect MovedToTextEffect

public RevisionTextEffect RevisedPropertiesEffect 
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




