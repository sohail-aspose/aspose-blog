---
title: 'Support of Mobi (Mobipocket) Document in Aspose.Words 16.8.0'
date: Wed, 21 Sep 2016 10:42:45 +0000
draft: false
url: /2016/09/21/support-of-mobi-mobipocket-document-in-aspose.words-16.8.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.8.0 has been released. This month’s release contains over 68 useful new features, enhancements and bug fixes to the Aspose.Words product.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.8.0][1]
*   [Aspose.Words for Java 16.8.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Support Loading of Mobi (Mobipocket) Document.
*   Added New Base Class FixedPageSaveOptions for all Fixed Page Formats e.g. PNG, PDF.
*   Hijri/Lunar, Hebrew Calendar Date Field option supported
*   The Analogue of NEXT Field is Added to LINQ Reporting Engine
*   Performance Optimization of UpdateFields and ExecuteWithRegions
*   Added HtmlLoadOptions.SupportVml Public Property
*   Added HtmlSaveOptions.ExportTextBoxAsSvg Public Property
*   HtmlLoadOptions Public Class is Introduced
*   Changes in Save Options of Fixed Page Formats

## Added HtmlLoadOptions.SupportVml Public Property

We have added the HtmlLoadOptions.SupportVml property in Aspose.Wrods v16.8.0 to specify HTML parser to parse conditional comments exactly like <!--\[if gte vml 1\]> and not to parse conditional comments exactly like <!\[if !vml\]>.

```
/// <summary>
/// Specifies HTML parser to parse conditional comments exactly like <! [if gte vml 1]>
/// and not to parse conditional comments exactly like <![if !vml]>.
/// </summary>
public bool SupportVml
{
    get { return mSupportVml; }
    set { mSupportVml = value; }
}
```

## Added HtmlSaveOptions.ExportTextBoxAsSvg Public Property

We have added the HtmlSaveOptions.ExportTextBoxAsSvg property in Aspose.Wrods v16.8.0 to control how textboxes represented by Shape are saved to HTML, MHTML or EPUB.

```
/// <summary>
/// Controls how textboxes represented by <see cref="Drawing.Shape"/> are saved to HTML, MHTML or EPUB. 
/// Default value is <c>false</c>.
/// </summary>
/// <remarks>
/// When set to <c>true</c>, exports textboxes as inline <b><svg></b> elements. 
/// When <c>false</c>, exports as <b><img></b> elements.
/// </remarks>
public bool ExportTextBoxAsSvg
{
    get { return mSaveImageOptions.TextBoxAsSvg; }
    set { mSaveImageOptions.TextBoxAsSvg = value; }
}
```

## Introduced HtmlLoadOptions Public Class

We have introduced new public class HtmlLoadOptions in Aspose.Words v16.8.0. This class is a subclass of LoadOptions and should be used instead of LoadOptions whenever specific options are needed to be set when loading HTML document. Currently HtmlLoadOptions class has two properties:

```
/// <summary>
/// Specifies HTML parser to parse conditional comments exactly like <!--[if gte vml 1]>
/// and not to parse conditional comments exactly like <![if !vml]>.
/// </summary>
public bool SupportVml
{
    get { return mSupportVml; }
    set { mSupportVml = value; }
}

/// <summary>
/// The number of milliseconds to wait before the web request times out. The default value is 100000 milliseconds (100 seconds).
/// </summary>
/// <remarks>
/// The number of milliseconds that Aspose.Words waits for a response, when loading external resources (images, style sheets)
/// linked in HTML and MHTML documents.
/// </remarks>
public new int WebRequestTimeout
{
    get { return mWebRequestTimeout; }
    set { mWebRequestTimeout = value; }
} 
```

Base property LoadOptions.WebRequestTimeout is marked as obsolete and will be removed in several releases. If you need to specify web request timeout use HtmlLoadOptions.WebRequestTimeout property.

Use case:

```
HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
htmlLoadOptions.SupportVml = true;
htmlLoadOptions.WebRequestTimeout = 1000;
Document doc = new Document("Test.html", htmlLoadOptions);
```

## Changes in Save Options of Fixed Page Formats

1\. Now all save option classes of fixed page formats (HtmlFixedSaveOptions, ImageSaveOptions, PdfSaveOptions, PsSaveOptions, SvgSaveOptions, SwfSaveOptions, XamlFixedSaveOptions and XpsSaveOptions) are inherited from the new public abstract class FixedPageSaveOptions.

2\. The MetafileRenderingOptions property has become available in the SwfSaveOptions class:

```
/// <summary>
/// Allows to specify metafile rendering options.
/// </summary>
public MetafileRenderingOptions MetafileRenderingOptions { get; }
```

3\. The JpegQuality property has become available in the XamlFixedSaveOptions and XpsSaveOptions classes:

```
/// <summary>
/// Gets or sets a value determining the quality of the JPEG images inside Html document.
/// </summary>
/// <remarks>
/// <para>Has effect only when a document contains JPEG images.</para>
///
/// Use this property to get or set the quality of the images inside a document when saving in fixed page format.
/// The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100
/// means best quality but minimum compression.
///
/// The default value is 95.
/// </remarks>
public int JpegQuality { get; set; } 
```

Jpeg quality was 100 for the XAML and XPS formats in the previous version. Now its default value is 95 to unify with the other formats (except PDF).

## Analogue of NEXT Fields is Added to LINQ Reporting Engine

We have introduced NEXT Field in LINQ Reporting Engine to force movement to next item within Data Band. Please refer to article : "Forcing Movement to Next Item within Data Band".




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




